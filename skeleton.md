# Skeleton Examples with Tailwind CSS

## Example 1: Basic Skeleton Elements
```html
<!-- Text Lines -->
<div class="space-y-2">
    <div class="h-4 bg-gray-200 rounded-md animate-pulse w-3/4"></div>
    <div class="h-4 bg-gray-200 rounded-md animate-pulse"></div>
    <div class="h-4 bg-gray-200 rounded-md animate-pulse w-5/6"></div>
    <div class="h-4 bg-gray-200 rounded-md animate-pulse w-4/5"></div>
</div>

<!-- Heading and Text -->
<div class="space-y-2 mt-6">
    <div class="h-6 bg-gray-200 rounded-md animate-pulse w-1/2"></div>
    <div class="h-4 bg-gray-200 rounded-md animate-pulse w-full"></div>
    <div class="h-4 bg-gray-200 rounded-md animate-pulse w-5/6"></div>
</div>

<!-- Shapes -->
<div class="flex flex-wrap gap-4">
    <div class="w-16 h-16 bg-gray-200 rounded-md animate-pulse"></div>
    <div class="w-16 h-16 bg-gray-200 rounded-full animate-pulse"></div>
    <div class="w-32 h-12 bg-gray-200 rounded-lg animate-pulse"></div>
</div>
```

## Example 2: Card Skeletons
```html
<!-- Product Card Skeleton -->
<div class="border border-gray-200 rounded-lg overflow-hidden">
    <div class="h-48 bg-gray-200 animate-pulse-custom"></div>
    <div class="p-4 space-y-3">
        <div class="h-5 bg-gray-200 rounded animate-pulse-custom w-2/3"></div>
        <div class="h-4 bg-gray-200 rounded animate-pulse-custom w-full"></div>
        <div class="h-4 bg-gray-200 rounded animate-pulse-custom w-4/5"></div>
        <div class="flex justify-between items-center pt-2">
            <div class="h-6 bg-gray-200 rounded animate-pulse-custom w-1/3"></div>
            <div class="h-8 bg-gray-200 rounded animate-pulse-custom w-24"></div>
        </div>
    </div>
</div>

<!-- Profile Card Skeleton -->
<div class="border border-gray-200 rounded-lg overflow-hidden">
    <div class="h-24 bg-gray-200 animate-pulse-custom"></div>
    <div class="flex justify-center">
        <div class="h-20 w-20 bg-gray-200 rounded-full -mt-10 border-4 border-white animate-pulse-custom"></div>
    </div>
    <div class="p-4 text-center space-y-3">
        <div class="h-5 bg-gray-200 rounded animate-pulse-custom w-1/2 mx-auto"></div>
        <div class="h-4 bg-gray-200 rounded animate-pulse-custom w-2/3 mx-auto"></div>
        <div class="flex justify-center gap-2 pt-2">
            <div class="h-8 w-8 bg-gray-200 rounded-full animate-pulse-custom"></div>
            <div class="h-8 w-8 bg-gray-200 rounded-full animate-pulse-custom"></div>
            <div class="h-8 w-8 bg-gray-200 rounded-full animate-pulse-custom"></div>
        </div>
    </div>
</div>
```

## Example 3: Shimmer Effect Skeletons
```html
<!-- List Item with Shimmer Effect -->
<div class="flex items-center space-x-4">
    <div class="h-12 w-12 bg-gray-200 rounded-full skeleton-wave"></div>
    <div class="flex-1 space-y-2">
        <div class="h-4 bg-gray-200 rounded skeleton-wave w-3/4"></div>
        <div class="h-3 bg-gray-200 rounded skeleton-wave w-1/2"></div>
    </div>
    <div class="h-8 w-8 bg-gray-200 rounded-full skeleton-wave"></div>
</div>

<!-- CSS for Shimmer Effect -->
<style>
    .skeleton-wave {
        position: relative;
        overflow: hidden;
    }
    
    .skeleton-wave::after {
        position: absolute;
        top: 0;
        right: 0;
        bottom: 0;
        left: 0;
        transform: translateX(-100%);
        background: linear-gradient(90deg, 
            rgba(255, 255, 255, 0) 0%, 
            rgba(255, 255, 255, 0.2) 50%, 
            rgba(255, 255, 255, 0) 100%);
        animation: shimmer 2s infinite;
        content: '';
    }

    @keyframes shimmer {
        0% {
            background-position: -200% 0;
        }
        100% {
            background-position: 200% 0;
        }
    }
</style>
```

## Example 4: Complex Page Layout Skeletons
```html
<!-- Dashboard Layout Skeleton (Sidebar) -->
<div class="md:col-span-3 space-y-4">
    <div class="h-8 bg-gray-200 rounded animate-pulse w-1/2"></div>
    <div class="space-y-2">
        <div class="h-10 bg-gray-200 rounded animate-pulse"></div>
        <div class="h-10 bg-gray-200 rounded animate-pulse"></div>
        <div class="h-10 bg-gray-200 rounded animate-pulse"></div>
        <div class="h-10 bg-gray-200 rounded animate-pulse"></div>
        <div class="h-10 bg-gray-200 rounded animate-pulse"></div>
    </div>
</div>

<!-- Stats Cards Skeleton -->
<div class="grid md:grid-cols-4 gap-4">
    <div class="border border-gray-200 rounded-lg p-4">
        <div class="h-4 bg-gray-200 rounded animate-pulse w-1/2 mb-2"></div>
        <div class="h-6 bg-gray-200 rounded animate-pulse w-1/3 mb-2"></div>
        <div class="h-2 bg-gray-200 rounded animate-pulse w-full"></div>
    </div>
    <!-- Repeat for additional cards -->
</div>

<!-- Chart Placeholder Skeleton -->
<div class="border border-gray-200 rounded-lg p-4">
    <div class="h-4 bg-gray-200 rounded animate-pulse w-1/3 mb-4"></div>
    <div class="h-60 bg-gray-200 rounded animate-pulse"></div>
</div>
```

## Example 5: Themed and Colored Skeletons
```html
<!-- Dark Theme Skeleton -->
<div class="bg-gray-800 p-4 rounded-lg">
    <h3 class="text-md font-medium text-gray-200 mb-4">Dark Theme</h3>
    <div class="space-y-3">
        <div class="h-4 bg-gray-600 rounded-md animate-pulse w-3/4"></div>
        <div class="h-4 bg-gray-600 rounded-md animate-pulse"></div>
        <div class="h-4 bg-gray-600 rounded-md animate-pulse w-5/6"></div>
        <div class="h-4 bg-gray-600 rounded-md animate-pulse w-4/5"></div>
        <div class="flex items-center space-x-3 mt-4">
            <div class="h-10 w-10 bg-gray-600 rounded-full animate-pulse"></div>
            <div class="flex-1 space-y-2">
                <div class="h-3 bg-gray-600 rounded animate-pulse"></div>
                <div class="h-3 bg-gray-600 rounded animate-pulse w-4/5"></div>
            </div>
        </div>
    </div>
</div>

<!-- Brand Colored Skeleton -->
<div class="bg-blue-50 p-4 rounded-lg border border-blue-100">
    <h3 class="text-md font-medium text-blue-800 mb-4">Brand Theme</h3>
    <div class="space-y-3">
        <div class="h-4 bg-blue-200 rounded-md animate-pulse w-3/4"></div>
        <div class="h-4 bg-blue-200 rounded-md animate-pulse"></div>
        <div class="h-4 bg-blue-200 rounded-md animate-pulse w-5/6"></div>
        <div class="h-4 bg-blue-200 rounded-md animate-pulse w-4/5"></div>
    </div>
</div>

<!-- Gradient Skeleton -->
<div class="bg-gradient-to-r from-purple-50 to-pink-50 p-4 rounded-lg border border-pink-100">
    <h3 class="text-md font-medium text-pink-800 mb-4">Gradient Theme</h3>
    <div class="space-y-3">
        <div class="h-4 bg-gradient-to-r from-purple-200 to-pink-200 rounded-md animate-pulse-custom w-3/4"></div>
        <div class="h-4 bg-gradient-to-r from-purple-200 to-pink-200 rounded-md animate-pulse-custom"></div>
        <div class="h-4 bg-gradient-to-r from-purple-200 to-pink-200 rounded-md animate-pulse-custom w-5/6"></div>
    </div>
</div>
```

## Interactive Demo JavaScript
```javascript
// Toggle between skeleton and content
document.getElementById('toggleSkeletonBtn').addEventListener('click', function() {
    const button = this;
    const skeletonState = document.getElementById('skeletonState');
    const contentState = document.getElementById('contentState');
    
    if (skeletonState.classList.contains('animate-pulse')) {
        // Show content
        skeletonState.classList.add('hidden');
        skeletonState.classList.remove('animate-pulse');
        contentState.classList.remove('hidden');
        
        button.textContent = 'Show Skeleton';
    } else {
        // Show skeleton
        skeletonState.classList.remove('hidden');
        skeletonState.classList.add('animate-pulse');
        contentState.classList.add('hidden');
        
        button.textContent = 'Show Content';
    }
});
```
