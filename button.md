# Button Component Examples

Collection of 5 beautiful button designs using Tailwind CSS and Remix Icons.

## Example 1 - Primary Action Button
Modern gradient button with icon and smooth hover effects.

```html
<button class="group relative inline-flex items-center justify-center px-8 py-3 text-lg font-medium text-white bg-gradient-to-r from-blue-600 to-blue-700 rounded-lg shadow-lg hover:shadow-xl transition-all duration-300 hover:scale-105 transform">
    <i class="ri-shopping-cart-line text-xl mr-3 group-hover:animate-pulse"></i>
    Add to Cart
    <div class="absolute inset-0 bg-gradient-to-r from-blue-700 to-blue-800 rounded-lg opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
    <span class="relative z-10">Add to Cart</span>
    <i class="ri-shopping-cart-line text-xl mr-3 relative z-10 group-hover:animate-pulse"></i>
</button>
```

## Example 2 - Outline Button
Clean outline design with animated icon and smooth transitions.

```html
<button class="group relative inline-flex items-center justify-center px-8 py-3 text-lg font-medium text-emerald-600 bg-transparent border-2 border-emerald-600 rounded-lg hover:bg-emerald-600 hover:text-white transition-all duration-300 hover:shadow-lg">
    <i class="ri-download-line text-xl mr-3 group-hover:translate-y-0.5 transition-transform duration-300"></i>
    Download
</button>
```

## Example 3 - Social Login Button
Eye-catching gradient button for social authentication.

```html
<button class="group relative inline-flex items-center justify-center w-full px-8 py-3 text-lg font-medium text-white bg-gradient-to-r from-purple-600 via-pink-600 to-red-600 rounded-lg shadow-lg hover:shadow-xl transition-all duration-300 hover:scale-105 transform">
    <i class="ri-google-fill text-xl mr-3"></i>
    Continue with Google
    <div class="absolute inset-0 bg-gradient-to-r from-purple-700 via-pink-700 to-red-700 rounded-lg opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
    <span class="relative z-10 flex items-center">
        <i class="ri-google-fill text-xl mr-3"></i>
        Continue with Google
    </span>
</button>
```

## Example 4 - Icon Action Buttons
Minimalist icon buttons with subtle hover effects.

```html
<div class="flex space-x-4">
    <button class="group relative inline-flex items-center justify-center w-12 h-12 text-gray-600 bg-gray-100 rounded-full hover:bg-red-500 hover:text-white transition-all duration-300 hover:scale-110 transform">
        <i class="ri-heart-line text-xl group-hover:ri-heart-fill"></i>
    </button>
    <button class="group relative inline-flex items-center justify-center w-12 h-12 text-gray-600 bg-gray-100 rounded-full hover:bg-blue-500 hover:text-white transition-all duration-300 hover:scale-110 transform">
        <i class="ri-share-line text-xl group-hover:animate-pulse"></i>
    </button>
    <button class="group relative inline-flex items-center justify-center w-12 h-12 text-gray-600 bg-gray-100 rounded-full hover:bg-green-500 hover:text-white transition-all duration-300 hover:scale-110 transform">
        <i class="ri-bookmark-line text-xl group-hover:ri-bookmark-fill"></i>
    </button>
</div>
```

## Example 5 - CTA Button with Badge
Call-to-action button with notification badge and glow effect.

```html
<button class="group relative inline-flex items-center justify-center px-8 py-4 text-lg font-semibold text-white bg-gradient-to-r from-orange-500 to-red-500 rounded-xl shadow-lg hover:shadow-2xl transition-all duration-300 hover:scale-105 transform">
    <i class="ri-notification-line text-xl mr-3 group-hover:animate-bounce"></i>
    Get Updates
    <span class="absolute -top-2 -right-2 inline-flex items-center justify-center w-6 h-6 text-xs font-bold text-orange-600 bg-white rounded-full border-2 border-orange-500 group-hover:animate-pulse">
        3
    </span>
    <div class="absolute inset-0 bg-gradient-to-r from-orange-600 to-red-600 rounded-xl opacity-0 group-hover:opacity-100 transition-opacity duration-300"></div>
    <span class="relative z-10 flex items-center">
        <i class="ri-notification-line text-xl mr-3 group-hover:animate-bounce"></i>
        Get Updates
    </span>
</button>
```

## Usage Notes

- All buttons use Tailwind CSS for styling
- Icons are from Remix Icons library
- Hover effects include smooth transitions and transforms
- No JavaScript required - pure CSS animations
- Responsive design with proper spacing
- Light theme optimized with clean aesthetics
