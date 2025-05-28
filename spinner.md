# Spinner Examples with Tailwind CSS

## Example 1: Basic Spinners
```html
<!-- Border Spinner -->
<div class="text-center">
    <div class="h-12 w-12 border-4 border-blue-500 border-t-transparent rounded-full custom-spin mx-auto"></div>
    <p class="mt-3 text-sm text-gray-600">Border Spinner</p>
</div>

<!-- Dotted Border Spinner -->
<div class="text-center">
    <div class="h-12 w-12 border-4 border-dotted border-purple-500 rounded-full custom-spin mx-auto"></div>
    <p class="mt-3 text-sm text-gray-600">Dotted Spinner</p>
</div>

<!-- Dashed Border Spinner -->
<div class="text-center">
    <div class="h-12 w-12 border-4 border-dashed border-green-500 rounded-full custom-spin mx-auto"></div>
    <p class="mt-3 text-sm text-gray-600">Dashed Spinner</p>
</div>

<!-- Icon Spinner -->
<div class="text-center">
    <i class="ri-loader-4-line text-4xl text-amber-500 custom-spin block"></i>
    <p class="mt-3 text-sm text-gray-600">Icon Spinner</p>
</div>

<!-- Dual Ring Spinner -->
<div class="text-center">
    <div class="relative h-12 w-12 mx-auto">
        <div class="absolute inset-0 border-4 border-t-pink-500 border-r-pink-500 border-b-transparent border-l-transparent rounded-full custom-spin"></div>
        <div class="absolute inset-0.5 border-4 border-t-transparent border-r-transparent border-b-pink-300 border-l-pink-300 rounded-full spin-slow"></div>
    </div>
    <p class="mt-3 text-sm text-gray-600">Dual Ring Spinner</p>
</div>
```

## Example 2: Colored Spinners with Different Sizes
```html
<!-- Small Spinner -->
<div class="text-center">
    <div class="h-6 w-6 border-2 border-red-600 border-t-transparent rounded-full custom-spin mx-auto"></div>
    <p class="mt-3 text-xs text-gray-600">Small</p>
</div>

<!-- Medium Spinner -->
<div class="text-center">
    <div class="h-8 w-8 border-2 border-yellow-600 border-t-transparent rounded-full custom-spin mx-auto"></div>
    <p class="mt-3 text-xs text-gray-600">Medium</p>
</div>

<!-- Large Spinner -->
<div class="text-center">
    <div class="h-12 w-12 border-4 border-green-600 border-t-transparent rounded-full custom-spin mx-auto"></div>
    <p class="mt-3 text-xs text-gray-600">Large</p>
</div>
```

## Example 3: Creative Spinners
```html
<!-- Pulse Dot Spinner -->
<div class="text-center">
    <div class="flex space-x-2 mx-auto justify-center">
        <div class="h-4 w-4 bg-indigo-600 rounded-full pulse-animation" style="animation-delay: 0s;"></div>
        <div class="h-4 w-4 bg-indigo-600 rounded-full pulse-animation" style="animation-delay: 0.3s;"></div>
        <div class="h-4 w-4 bg-indigo-600 rounded-full pulse-animation" style="animation-delay: 0.6s;"></div>
    </div>
    <p class="mt-3 text-sm text-gray-600">Pulse Dots</p>
</div>

<!-- Bouncing Balls -->
<div class="text-center">
    <div class="flex space-x-2 mx-auto justify-center h-10">
        <div class="h-3 w-3 bg-green-500 rounded-full bounce-animation" style="animation-delay: 0s;"></div>
        <div class="h-3 w-3 bg-green-500 rounded-full bounce-animation" style="animation-delay: 0.2s;"></div>
        <div class="h-3 w-3 bg-green-500 rounded-full bounce-animation" style="animation-delay: 0.4s;"></div>
        <div class="h-3 w-3 bg-green-500 rounded-full bounce-animation" style="animation-delay: 0.6s;"></div>
    </div>
    <p class="mt-3 text-sm text-gray-600">Bouncing Balls</p>
</div>

<!-- Growing Circle -->
<div class="text-center">
    <div class="h-12 w-12 bg-pink-500 rounded-full grow-shrink mx-auto opacity-75"></div>
    <p class="mt-3 text-sm text-gray-600">Growing Circle</p>
</div>
```

## Example 4: SVG Spinners
```html
<!-- Circular Progress -->
<div class="text-center">
    <svg class="mx-auto" width="60" height="60" viewBox="0 0 50 50">
        <circle cx="25" cy="25" r="20" fill="none" stroke="#e6e6e6" stroke-width="4"></circle>
        <circle class="progress-ring__circle dash-animation" cx="25" cy="25" r="20" fill="none" stroke="#3B82F6" stroke-width="4"></circle>
    </svg>
    <p class="mt-3 text-sm text-gray-600">Circular Progress</p>
</div>

<!-- Spinning Wheel -->
<div class="text-center">
    <svg class="mx-auto custom-spin" width="60" height="60" viewBox="0 0 24 24">
        <circle cx="12" cy="12" r="10" fill="none" stroke="#e6e6e6" stroke-width="2"></circle>
        <path d="M12 2 a10 10 0 0 1 10 10" fill="none" stroke="#8B5CF6" stroke-width="2" stroke-linecap="round"></path>
    </svg>
    <p class="mt-3 text-sm text-gray-600">Spinning Wheel</p>
</div>

<!-- Bars Spinner -->
<div class="text-center">
    <svg class="mx-auto" width="60" height="50" viewBox="0 0 120 30">
        <rect class="pulse-animation" x="15" y="10" width="10" height="30" fill="#10B981" style="animation-delay: 0s;"></rect>
        <rect class="pulse-animation" x="35" y="10" width="10" height="30" fill="#10B981" style="animation-delay: 0.2s;"></rect>
        <rect class="pulse-animation" x="55" y="10" width="10" height="30" fill="#10B981" style="animation-delay: 0.4s;"></rect>
        <rect class="pulse-animation" x="75" y="10" width="10" height="30" fill="#10B981" style="animation-delay: 0.6s;"></rect>
        <rect class="pulse-animation" x="95" y="10" width="10" height="30" fill="#10B981" style="animation-delay: 0.8s;"></rect>
    </svg>
    <p class="mt-3 text-sm text-gray-600">Equalizer Bars</p>
</div>
```

## Example 5: Contextual Spinners with Messages
```html
<!-- Loading Button Spinner -->
<button class="bg-blue-600 hover:bg-blue-700 text-white font-medium rounded-lg text-sm px-6 py-3 flex items-center space-x-2 focus:outline-none focus:ring-4 focus:ring-blue-300">
    <svg class="animate-spin h-5 w-5 text-white" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
        <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
        <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
    </svg>
    <span>Processing Payment...</span>
</button>

<!-- Fullscreen Loading Overlay -->
<div class="relative w-full max-w-md h-48 border border-gray-200 rounded-lg overflow-hidden">
    <div class="absolute inset-0 bg-white bg-opacity-80 flex flex-col items-center justify-center">
        <div class="h-12 w-12 border-4 border-indigo-500 border-t-transparent rounded-full custom-spin"></div>
        <p class="mt-3 text-indigo-700 font-medium">Loading Dashboard...</p>
    </div>
    <div class="p-4 opacity-20 pointer-events-none">
        <!-- Content that is loading -->
    </div>
</div>
```

## CSS for Spinner Animations
```css
/* Custom spinning animations */
@keyframes spin {
    to {
        transform: rotate(360deg);
    }
}

@keyframes pulse-scale {
    0%, 100% {
        transform: scale(0.8);
        opacity: 0.8;
    }
    50% {
        transform: scale(1);
        opacity: 1;
    }
}

@keyframes grow-shrink {
    0%, 100% {
        transform: scale(0.5);
    }
    50% {
        transform: scale(1);
    }
}

@keyframes dash {
    to {
        stroke-dashoffset: 0;
    }
}

@keyframes bounce-loader {
    0%, 100% {
        transform: translateY(0);
    }
    50% {
        transform: translateY(-15px);
    }
}

.custom-spin {
    animation: spin 1s linear infinite;
}

.spin-slow {
    animation: spin 2s linear infinite;
}

.spin-fast {
    animation: spin 0.5s linear infinite;
}

.pulse-animation {
    animation: pulse-scale 1.5s ease-in-out infinite;
}

.grow-shrink {
    animation: grow-shrink 1.5s ease-in-out infinite;
}

.dash-animation {
    stroke-dasharray: 90;
    stroke-dashoffset: 90;
    animation: dash 1.5s linear infinite alternate;
}

.bounce-animation {
    animation: bounce-loader 0.8s ease-in-out infinite;
}
```
