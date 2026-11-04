# SeekMake for Claude

SeekMake is the instant quoting and ordering platform manufacturing shops (3D printing, CNC machining, sheet metal) use to quote and sell parts. This plugin lets a shop owner run their SeekMake account from a conversation with Claude.

## What it does

- **Quotes and orders**: find a quote or order by its number or the customer's email, read its parts and prices, and get download links for its 3D files.
- **The shop's setup**: see its machines and the materials each one runs, with their prices, and how each technology is priced.
- **Pricing**: price a part the way the shop's instant quote does, from an attached STEP or STL file or from an existing quote.
- **Changes, with your confirmation**: create and send quotes, update a quote's status, prices or tracking, and set the shop up (technologies, machines, materials, pricing, taxes, discounts, shipping, profile). Claude restates every change and waits for you to confirm before anything is changed or emailed.

## Use it

Install the plugin, then connect the SeekMake connector from the plugin's **Connectors** tab and sign in with your SeekMake account. Then ask, for example:

- "How many quote requests did my shop get this week?"
- "What materials do we offer for 3D printing, and at what price?"
- "What would this part cost in PLA, 10 pieces?" (with the file attached)

## Data

The plugin contains one skill and a reference to SeekMake's MCP server at `https://api-v2.seekmake.com/api/public/v1/mcp/protocol`. Everything it reads or changes goes between Claude and your own SeekMake shop through that server, after you sign in with OAuth; you only ever see your own shop's data. The plugin itself stores nothing and sends data nowhere else.

- Privacy policy: https://seekmake.com/privacy-policy
- Terms: https://seekmake.com/terms-and-conditions
- Support: https://seekmake.com/contact-us
- Developer documentation: https://seekmake.com/developers-portal/api-docs
