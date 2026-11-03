# Douceur by Terry — Project Requirements

## Project summary

Build a mobile-friendly online storefront for Douceur by Terry, a bakery and treats business. The storefront will present the products and prices from the supplied menus. Customers can choose product options, add products to a cart, and send the order details to the business through WhatsApp.

## Goals

- Make the menu easy to browse on phones and computers.
- Show products, available options, and prices in Ghana cedis (GH₵).
- Let customers review a cart before sending an order.
- Make it clear that pickup or delivery details and payment are confirmed with the business.
- Provide contact information for events and catering.

## Audience and intended use

Customers who want to browse Douceur by Terry's baked goods, drinks, and ice cream, then contact the business to arrange an order.

## Brand and design direction

- Use the supplied Douceur by Terry menus as the visual reference.
- Use a warm cream and terracotta palette with an elegant, bakery-appropriate style.
- Start with attractive image placeholders; replace them with approved product photographs when available.
- Keep navigation, product choices, cart controls, and text usable on small screens.

## Storefront requirements

1. Show the business name and a clear way to browse the menu.
2. Organize products into cookies, banana bread, Ghanaian pies, milkshakes, lemonades, and ice cream.
3. Show the size or package choices and the matching price for each product.
4. Let customers select product options and quantities and add them to a cart.
5. Let customers review and remove or adjust cart items before ordering.
6. Create a WhatsApp message containing the selected products, options, quantities, and item totals. The customer sends the message to place an order request.
7. Show the listed business contact number, `055 942 0935`, and the social handles `@douceur.gh` and `@terry_fynn`.
8. Include an events-and-catering contact section.
9. Do not invent delivery coverage, delivery fees, stock availability, or preparation times. Customers confirm these details with the business.

## Menu content supplied

Prices below are in Ghana cedis (GH₵).

### Cookies

| Product | Option | Price |
|---|---|---:|
| Oat Chocolate Crunch | 1 | GH₵ 10 |
| Oat Chocolate Crunch | Pack of 3 | GH₵ 28 |
| Oat Chocolate Crunch | Pack of 6 | GH₵ 55 |
| Oat Chocolate Crunch | Pack of 12 | GH₵ 105 |
| So Tee Classic (Chocolate Chip) | 1 | GH₵ 12 |
| So Tee Classic (Chocolate Chip) | Pack of 3 | GH₵ 34 |
| So Tee Classic (Chocolate Chip) | Pack of 6 | GH₵ 66 |
| So Tee Classic (Chocolate Chip) | Pack of 12 | GH₵ 126 |
| Coconut Toffee | 1 | GH₵ 12 |
| Coconut Toffee | Pack of 3 | GH₵ 34 |
| Coconut Toffee | Pack of 6 | GH₵ 66 |
| Coconut Toffee | Pack of 12 | GH₵ 126 |

### Banana bread

| Product | Option | Price |
|---|---|---:|
| Classic Banana Bread | Slice | GH₵ 12 |
| Classic Banana Bread | Small loaf | GH₵ 50 |
| Classic Banana Bread | Large loaf | GH₵ 90 |
| Chocolate Chip / Biscoff | Small loaf | GH₵ 60 |
| Chocolate Chip / Biscoff | Large loaf | GH₵ 100 |
| Bana-Nuts (variety of nuts banana bread) | Small loaf | GH₵ 65 |
| Bana-Nuts (variety of nuts banana bread) | Large loaf | GH₵ 105 |

### Ghanaian pies

| Product | Price |
|---|---:|
| Meat Pie | GH₵ 15 |
| Fish Pie | GH₵ 15 |

### Milkshakes

| Product | Option | Price |
|---|---|---:|
| Oreo Crumble Dream | 350 ml | GH₵ 35 |
| Oreo Crumble Dream | 500 ml | GH₵ 45 |
| Biscoff Bliss | 350 ml | GH₵ 35 |
| Biscoff Bliss | 500 ml | GH₵ 45 |
| Berry Blast | 350 ml | GH₵ 40 |
| Berry Blast | 500 ml | GH₵ 50 |

### Lemonades

| Product | Option | Price |
|---|---|---:|
| Sunshine Squeeze (peach) | 350 ml | GH₵ 20 |
| Sunshine Squeeze (peach) | 500 ml | GH₵ 25 |
| Berry & Blush (strawberry) | 350 ml | GH₵ 20 |
| Berry & Blush (strawberry) | 500 ml | GH₵ 25 |
| Tea-Tee (tamarind) | 350 ml | GH₵ 20 |
| Tea-Tee (tamarind) | 500 ml | GH₵ 25 |

### Ice cream

| Product/flavour | Option | Price |
|---|---|---:|
| Vanilla or Chocolate | 1.5 L tub | GH₵ 180 |
| Velvet Crush | 1.5 L tub | GH₵ 190 |
| Vanilla Cookie Chip | 1.5 L tub | GH₵ 190 |
| Oreos & Cream | 1.5 L tub | GH₵ 190 |
| Berry Fusion | 1.5 L tub | GH₵ 190 |
| Butterscotch | 1.5 L tub | GH₵ 190 |
| Vanilla or Chocolate | 500 ml | GH₵ 65 |
| Other flavours | 500 ml | GH₵ 70 |

## Order and payment flow

- The first version uses a cart-to-WhatsApp handoff.
- The website does not process payments. Customers arrange payment on delivery or pickup with the business.
- Pickup/delivery availability, address, fees, and order acceptance are confirmed directly with the business.
- The business confirmed that `055 942 0935` is the WhatsApp order number. The WhatsApp link uses Ghana's international dialing code and removes the local leading zero: `233559420935`.

## Recommended technology

- **React** for the interactive storefront and cart.
- **TypeScript** to catch common coding mistakes while building.
- **Vite** to run the project during development and create the production website files.
- **CSS** for the responsive visual design.
- Browser storage may be used to retain a customer's cart on their device. It is not a shared order database.
- A static hosting provider can publish the frontend. A custom backend and database are not required for the agreed first version.

## Out of scope for the first version

- Online card or mobile-money payments.
- Customer accounts, order history, staff administration, or inventory management.
- A backend, database, automatic order processing, delivery dispatch, or automated order confirmation.
- Guaranteed delivery zones, fees, availability, or preparation times.

These features would require additional requirements and, where applicable, a separately deployed and configured backend, database, and payment provider. Publishing the frontend alone does not provide those services.

## Acceptance criteria

- The menu can be browsed on mobile and desktop.
- Product options display the prices supplied above.
- Customers can add products and options to a cart, change quantities, and review the total.
- The WhatsApp action includes the cart contents in a message and opens the correct business contact after its number is confirmed.
- The site does not imply that an order was paid for, accepted, or stored by the website.
- Events and catering contact details are visible.
- The final public website is tested through its deployed URL before launch is considered complete.

## Items to confirm before launch

- Provide approved product photographs and any final logo files, if available.
- Confirm the pickup location, delivery areas, and any fees to display (if desired).
- Choose a hosting provider and connect a domain if a custom domain is desired.
