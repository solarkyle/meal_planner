# Meal Planner

A clean, interactive meal planning app for weekly meal preparation. Features include drag-and-drop meal scheduling, macro tracking, shopping list generation, and a customizable meal repository.

## Features

- **Drag-and-drop Interface**: Easily plan your weekly meals with a simple drag-and-drop interface
- **Macro Tracking**: Monitor your daily and weekly macronutrient intake
- **Shopping List Generation**: Automatically create shopping lists based on your meal plan
- **Meal Repository**: Browse and search a collection of meals with nutrition information
- **Multiple Themes**: Choose between light, dark, and kawaii (pink) themes
- **Responsive Design**: Works on both desktop and mobile devices
- **Persistent Storage**: Saves your meal plans using localStorage

## How to Use

1. **Browse Meals**: Scroll through the meal repository at the bottom of the page
2. **Filter Meals**: Use the category buttons to filter breakfast, lunch, dinner, and snacks
3. **Add to Calendar**: Drag meals onto the weekly calendar
4. **Track Macros**: View daily and weekly macro totals that update automatically
5. **Generate Shopping List**: Click "Shopping List" to see all ingredients needed for the week
6. **Customize Goals**: Set your macro goals using the "Set Macro Goals" button

## Project Structure

This project is designed to be simple and easy to maintain:

- `index.html`: Contains all HTML, CSS, and JavaScript in a single file
- `meals.json`: Stores the meal data
- `images/`: Directory for meal images

## Customizing the Meal Repository

To add your own meals to the repository:

1. Fork this repository
2. Add meal images to the `images/` folder
3. Edit the `meals.json` file to add your own meals
4. Commit and push your changes

Follow this format when adding meals to `meals.json`:

```json
{
  "id": "m100",
  "name": "Your Meal Name",
  "image": "images/your-meal-image.jpg",
  "category": "breakfast",
  "macros": {
    "calories": 350,
    "protein": 20,
    "carbs": 35,
    "fat": 15,
    "fiber": 6
  },
  "ingredients": [
    "Ingredient 1",
    "Ingredient 2",
    "Ingredient 3",
    "Ingredient 4"
  ]
}
```

## Development

This application uses no build tools or frameworks - just vanilla JavaScript. To run it locally:

1. Clone the repository
2. Open `index.html` in your browser
3. Make changes as needed
4. Refresh to see your changes

If images are missing, the app will automatically generate colored placeholders based on meal categories.

## Deployment

The app is designed to work perfectly with GitHub Pages:

1. Push your repository to GitHub
2. Go to Settings > Pages
3. Set the source to your main branch
4. Click Save

Your meal planner will be live at `https://solarkyle.github.io/meal_planner/`

## Implementation Details

- **Single File Design**: All code is in one HTML file for simplicity
- **LocalStorage**: User data is saved in the browser's localStorage
- **JSON Data**: Meal information is loaded from a separate meals.json file
- **No Dependencies**: No external JavaScript libraries are used
- **Placeholder Images**: Automatically generates colored placeholders for missing images

## License

This project is open source and available under the MIT License.
