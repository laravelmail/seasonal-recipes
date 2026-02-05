# Seasonal Recipes

Professional newsletter showcasing seasonal recipes for the upcoming festive period.

![Thumbnail](./thumbnail.png)

## Template Details

- **Industries:** Food & Beverage
- **Message Type:** Newsletter
- **Tags:** holiday, cooking, seasonal recipes, meals, festive

## Files
- `index.html`: The improved, localized, and branded HTML template.
- `template.blade.php`: Ready-to-use Laravel Blade template with `asset()` helpers.
- `assets/`: Directory containing localized images and styles used in the template.

## Usage in Laravel

### 1. Store the Template
Place the `index.html` content in a Blade view (e.g., `resources/views/emails/seasonal-recipes.blade.php`).

### 2. Handle Assets
Move the content of `assets/` to your public directory (e.g., `public/vendor/mail-templates/seasonal-recipes/`) and update the paths in the HTML to use the `asset()` helper.

### 3. Send Email
```php
Mail::to($user)->send(new \App\Mail\GenericEmail([
    'view' => 'emails.seasonal-recipes',
    'data' => [
        // Your dynamic data here
    ]
]));
```

---
*Created with ❤️ by **[LaravelMail.com](https://laravelmail.com)** - Your source for professional email templates.*
