# Tooltip Examples with Tailwind CSS and Remix Icon

## Example 1: Basic Tooltips

```html
<!-- Top Tooltip -->
<div class="relative flex flex-col items-center group">
    <button class="px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-300">
        Hover Me (Top)
    </button>
    <div class="absolute bottom-full mb-2 hidden group-hover:flex flex-col items-center">
        <div class="whitespace-nowrap px-3 py-2 bg-gray-900 text-white text-sm rounded-lg">
            Tooltip on top
        </div>
        <div class="w-3 h-3 -mt-1.5 rotate-45 bg-gray-900"></div>
    </div>
</div>

<!-- Right Tooltip -->
<div class="relative flex items-center group">
    <button class="px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-300">
        Hover Me (Right)
    </button>
    <div class="absolute left-full ml-2 hidden group-hover:flex items-center">
        <div class="w-3 h-3 -ml-1.5 rotate-45 bg-gray-900"></div>
        <div class="whitespace-nowrap px-3 py-2 bg-gray-900 text-white text-sm rounded-lg">
            Tooltip on right
        </div>
    </div>
</div>
```

## Example 2: Styled Tooltips

```html
<!-- Info Tooltip -->
<div class="relative flex flex-col items-center group">
    <button class="px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-300 flex items-center">
        <i class="ri-information-line mr-2"></i> Info Tooltip
    </button>
    <div class="absolute bottom-full mb-2 hidden group-hover:flex flex-col items-center animate-fade-in">
        <div class="flex items-center gap-2 whitespace-nowrap px-4 py-2 bg-blue-600 text-white text-sm rounded-lg max-w-xs">
            <i class="ri-information-line text-lg"></i>
            <span>This is an informational message with additional details.</span>
        </div>
        <div class="w-3 h-3 -mt-1.5 rotate-45 bg-blue-600"></div>
    </div>
</div>

<!-- Success Tooltip -->
<div class="relative flex flex-col items-center group">
    <button class="px-4 py-2 bg-green-500 text-white rounded-lg hover:bg-green-600 focus:outline-none focus:ring-2 focus:ring-green-300 flex items-center">
        <i class="ri-check-line mr-2"></i> Success Tooltip
    </button>
    <div class="absolute bottom-full mb-2 hidden group-hover:flex flex-col items-center animate-fade-in">
        <div class="flex items-center gap-2 whitespace-nowrap px-4 py-2 bg-green-600 text-white text-sm rounded-lg max-w-xs">
            <i class="ri-check-line text-lg"></i>
            <span>Operation completed successfully!</span>
        </div>
        <div class="w-3 h-3 -mt-1.5 rotate-45 bg-green-600"></div>
    </div>
</div>
```

## Example 3: Interactive Tooltips

```html
<!-- Tooltip with Link -->
<div class="relative flex flex-col items-center group">
    <button class="px-4 py-2 bg-purple-500 text-white rounded-lg hover:bg-purple-600 focus:outline-none focus:ring-2 focus:ring-purple-300">
        Help
    </button>
    <div class="absolute bottom-full mb-2 hidden group-hover:block animate-fade-in z-10">
        <div class="bg-white border border-gray-200 rounded-lg shadow-lg p-4 max-w-xs">
            <h3 class="font-medium text-gray-900">Need assistance?</h3>
            <p class="text-sm text-gray-600 mt-2">Visit our help center for more information.</p>
            <div class="mt-3">
                <a href="#" class="text-sm text-purple-600 hover:text-purple-800 font-medium flex items-center">
                    Learn more
                    <i class="ri-arrow-right-line ml-1"></i>
                </a>
            </div>
        </div>
        <div class="w-3 h-3 bg-white border-b border-r border-gray-200 -mb-1.5 rotate-45 mx-auto"></div>
    </div>
</div>

<!-- Click to Show Tooltip -->
<div class="relative flex flex-col items-center">
    <button id="click-tooltip-btn" class="px-4 py-2 bg-indigo-500 text-white rounded-lg hover:bg-indigo-600 focus:outline-none focus:ring-2 focus:ring-indigo-300">
        Click Me
    </button>
    <div id="click-tooltip" class="absolute bottom-full mb-2 hidden animate-fade-in z-10">
        <div class="bg-white border border-gray-200 rounded-lg shadow-lg p-4 max-w-xs">
            <h3 class="font-medium text-gray-900 flex items-center">
                <i class="ri-lightbulb-line text-yellow-500 mr-2"></i>
                Did you know?
            </h3>
            <p class="text-sm text-gray-600 mt-2">This tooltip is triggered by a click instead of hover.</p>
            <div class="mt-3 text-right">
                <button id="close-tooltip-btn" class="text-xs bg-gray-200 hover:bg-gray-300 px-2 py-1 rounded">
                    Close
                </button>
            </div>
        </div>
        <div class="w-3 h-3 bg-white border-b border-r border-gray-200 -mb-1.5 rotate-45 mx-auto"></div>
    </div>
</div>
```

## Example 4: Tooltip Transitions and Animations

```html
<!-- Fade In Tooltip -->
<div class="relative flex flex-col items-center group">
    <button class="px-4 py-2 bg-blue-500 text-white rounded-lg hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-300">
        Fade In
    </button>
    <div class="absolute bottom-full mb-2 opacity-0 group-hover:opacity-100 transition-opacity duration-300 flex flex-col items-center">
        <div class="whitespace-nowrap px-3 py-2 bg-gray-900 text-white text-sm rounded-lg">
            Fades in smoothly
        </div>
        <div class="w-3 h-3 -mt-1.5 rotate-45 bg-gray-900"></div>
    </div>
</div>

<!-- Scale Tooltip -->
<div class="relative flex flex-col items-center group">
    <button class="px-4 py-2 bg-green-500 text-white rounded-lg hover:bg-green-600 focus:outline-none focus:ring-2 focus:ring-green-300">
        Scale Effect
    </button>
    <div class="absolute bottom-full mb-2 scale-0 group-hover:scale-100 transition-transform duration-300 origin-bottom flex flex-col items-center">
        <div class="whitespace-nowrap px-3 py-2 bg-gray-900 text-white text-sm rounded-lg">
            Scales in and out
        </div>
        <div class="w-3 h-3 -mt-1.5 rotate-45 bg-gray-900"></div>
    </div>
</div>
```

## Example 5: Custom Tooltips

```html
<!-- Custom Form Field Tooltip -->
<div class="relative">
    <label for="password" class="block mb-2 text-sm font-medium text-gray-900">
        Password
        <span class="ml-1 text-gray-500 cursor-help group relative inline-block">
            <i class="ri-question-line"></i>
            <span class="opacity-0 invisible group-hover:opacity-100 group-hover:visible absolute left-full ml-2 bottom-0 z-10 w-64 bg-white border border-gray-200 rounded-lg shadow-lg p-3 text-xs text-gray-500 transition-opacity duration-300">
                Password must be at least 8 characters long and include:
                <ul class="mt-1 list-disc list-inside">
                    <li>One uppercase letter</li>
                    <li>One lowercase letter</li>
                    <li>One number</li>
                    <li>One special character (e.g. !@#$%^&*)</li>
                </ul>
            </span>
        </span>
    </label>
    <input type="password" id="password" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
</div>

<!-- Chart Value Tooltip -->
<div class="relative group">
    <div class="h-40 bg-gray-100 rounded-lg w-72 p-4 flex items-end justify-between">
        <div class="relative h-32 w-8 bg-blue-200 rounded">
            <div class="absolute bottom-0 h-16 w-8 bg-blue-500 rounded"></div>
            <span class="absolute -top-7 left-0 w-8 text-center text-xs font-medium text-gray-500">Jan</span>
            <div class="absolute -top-4 left-0 w-8 text-center opacity-0 group-hover:opacity-100 transition-opacity">
                <div class="tooltip-arrow arrow-top relative inline-block px-2 py-1 bg-black text-white text-xs rounded">
                    45%
                </div>
            </div>
        </div>
        <!-- Additional chart bars -->
    </div>
</div>
```

### JavaScript for Interactive Tooltips

```javascript
// Click tooltip functionality
const clickTooltipBtn = document.getElementById('click-tooltip-btn');
const clickTooltip = document.getElementById('click-tooltip');
const closeTooltipBtn = document.getElementById('close-tooltip-btn');

clickTooltipBtn.addEventListener('click', () => {
    clickTooltip.classList.toggle('hidden');
});

closeTooltipBtn.addEventListener('click', () => {
    clickTooltip.classList.add('hidden');
});

// Bounce tooltip functionality
const bounceTooltipBtn = document.getElementById('bounce-tooltip-btn');
const bounceTooltip = document.getElementById('bounce-tooltip');

bounceTooltipBtn.addEventListener('mouseenter', () => {
    bounceTooltip.classList.remove('hidden');
    bounceTooltip.animate([
        { transform: 'translateY(0)', opacity: 0 },
        { transform: 'translateY(-5px)', opacity: 1 },
        { transform: 'translateY(0)', opacity: 1 },
        { transform: 'translateY(-2px)', opacity: 1 },
        { transform: 'translateY(0)', opacity: 1 }
    ], {
        duration: 500,
        easing: 'ease-out'
    });
});
```
