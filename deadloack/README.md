# Deadlock Items Website

This website displays items from the game Deadlock, organized by category (Weapons, Vitality, and Spirit) and price tiers.

## Features

- Browse items by category and price tier
- View detailed item information on hover
- See related items highlighted when hovering over an item
- Responsive design for all screen sizes

## Files Structure

- `index.html` - Weapons items page
- `vitality.html` - Vitality items page
- `spirit.html` - Spirit items page
- `images/` - Directory containing all item images

## Item Relationships

The website features an item relationship system that highlights related items when hovering over an item. These relationships are defined directly within each HTML file:

- `index.html`: Contains relationships between weapon items
- `vitality.html`: Contains relationships between vitality items
- `spirit.html`: Contains relationships between spirit items

Each file contains a JavaScript object with key-value pairs where:
- The key is the item name
- The value is an array of related item names

## How It Works

1. When a page loads, it uses the relationship data embedded in the HTML
2. When a user hovers over an item, the page highlights that item and all related items
3. All other items are dimmed to make the relationships more visible

## Hosting Requirements

This website requires a web server that can serve static files. No server-side processing is required.

## Browser Compatibility

The website is compatible with all modern browsers:
- Chrome
- Firefox
- Safari
- Edge

## Updating Relationships

To update item relationships, edit the JavaScript object in each HTML file. The structure looks like this:

```javascript
let itemRelationships = {
    "Item Name": ["Related Item 1", "Related Item 2", "Related Item 3"],
    // more items...
};
```

No admin panel is required - just update the HTML files and upload them to your web server. 