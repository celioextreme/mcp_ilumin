# Toast Examples with Tailwind CSS and Remix Icon

## Example 1: Simple Toast Notifications

```html
<!-- Success Toast -->
<div id="toast-success" class="flex items-center w-full max-w-xs p-4 mb-4 text-gray-500 bg-white rounded-lg shadow" role="alert">
    <div class="inline-flex items-center justify-center flex-shrink-0 w-8 h-8 text-green-500 bg-green-100 rounded-lg">
        <i class="ri-check-line"></i>
    </div>
    <div class="ml-3 text-sm font-normal">Item has been successfully added.</div>
    <button type="button" class="ml-auto -mx-1.5 -my-1.5 bg-white text-gray-400 hover:text-gray-900 rounded-lg p-1.5 hover:bg-gray-100 inline-flex h-8 w-8" data-dismiss-target="#toast-success" aria-label="Close">
        <span class="sr-only">Close</span>
        <i class="ri-close-line w-5 h-5"></i>
    </button>
</div>

<!-- Warning Toast -->
<div id="toast-warning" class="flex items-center w-full max-w-xs p-4 text-gray-500 bg-white rounded-lg shadow" role="alert">
    <div class="inline-flex items-center justify-center flex-shrink-0 w-8 h-8 text-yellow-500 bg-yellow-100 rounded-lg">
        <i class="ri-error-warning-line"></i>
    </div>
    <div class="ml-3 text-sm font-normal">You are approaching your usage limit.</div>
    <button type="button" class="ml-auto -mx-1.5 -my-1.5 bg-white text-gray-400 hover:text-gray-900 rounded-lg p-1.5 hover:bg-gray-100 inline-flex h-8 w-8" data-dismiss-target="#toast-warning" aria-label="Close">
        <span class="sr-only">Close</span>
        <i class="ri-close-line w-5 h-5"></i>
    </button>
</div>
```

## Example 2: Colored Toast Messages

```html
<!-- Info Toast -->
<div class="flex items-center p-4 text-blue-800 rounded-lg bg-blue-50" role="alert">
    <i class="ri-information-line flex-shrink-0 w-5 h-5"></i>
    <div class="ml-3 text-sm font-medium">
        A new software update is available. <a href="#" class="font-semibold underline hover:text-blue-900">Check it out</a>.
    </div>
    <button type="button" class="ml-auto -mx-1.5 -my-1.5 bg-blue-50 text-blue-500 rounded-lg p-1.5 hover:bg-blue-100 inline-flex h-8 w-8">
        <span class="sr-only">Close</span>
        <i class="ri-close-line w-5 h-5"></i>
    </button>
</div>

<!-- Success Toast -->
<div class="flex items-center p-4 mb-4 text-green-800 rounded-lg bg-green-50" role="alert">
    <i class="ri-checkbox-circle-line flex-shrink-0 w-5 h-5"></i>
    <div class="ml-3 text-sm font-medium">
        Your changes have been saved successfully!
    </div>
    <button type="button" class="ml-auto -mx-1.5 -my-1.5 bg-green-50 text-green-500 rounded-lg p-1.5 hover:bg-green-100 inline-flex h-8 w-8">
        <span class="sr-only">Close</span>
        <i class="ri-close-line w-5 h-5"></i>
    </button>
</div>
```

## Example 3: Toast with Action Buttons

```html
<!-- Undo Action Toast -->
<div id="toast-undo" class="w-full max-w-xs p-4 text-gray-500 bg-white rounded-lg shadow" role="alert">
    <div class="flex">
        <div class="inline-flex items-center justify-center flex-shrink-0 w-8 h-8 text-blue-500 bg-blue-100 rounded-lg">
            <i class="ri-delete-bin-line"></i>
        </div>
        <div class="ml-3 text-sm font-normal">
            <span class="mb-1 text-sm font-semibold text-gray-900">Item deleted</span>
            <div class="mb-2 text-sm font-normal">The item has been moved to trash.</div>
            <div class="grid grid-cols-2 gap-2">
                <div>
                    <button class="inline-flex justify-center w-full px-2 py-1.5 text-xs font-medium text-center text-white bg-blue-600 rounded-lg hover:bg-blue-700 focus:ring-4 focus:outline-none focus:ring-blue-300">Undo</button>
                </div>
                <div>
                    <button class="inline-flex justify-center w-full px-2 py-1.5 text-xs font-medium text-center text-gray-900 bg-white border border-gray-300 rounded-lg hover:bg-gray-100 focus:ring-4 focus:outline-none focus:ring-gray-200">Dismiss</button>
                </div>
            </div>
        </div>
        <button type="button" class="ml-auto -mx-1.5 -my-1.5 bg-white text-gray-400 hover:text-gray-900 rounded-lg p-1.5 hover:bg-gray-100 inline-flex h-8 w-8" data-dismiss-target="#toast-undo" aria-label="Close">
            <span class="sr-only">Close</span>
            <i class="ri-close-line w-5 h-5"></i>
        </button>
    </div>
</div>
```

## Example 4: Toast Positions

```html
<!-- Position Examples -->
<div class="relative h-64 border border-dashed border-gray-300 rounded-lg p-4 overflow-hidden">
    <!-- Top Left -->
    <div class="absolute top-4 left-4 flex items-center w-60 max-w-xs p-4 space-x-4 text-gray-500 bg-white divide-x divide-gray-200 rounded-lg shadow" role="alert">
        <i class="ri-information-line text-blue-600"></i>
        <div class="pl-4 text-sm font-normal">Top Left Position</div>
    </div>
    
    <!-- Top Right -->
    <div class="absolute top-4 right-4 flex items-center w-60 max-w-xs p-4 space-x-4 text-gray-500 bg-white divide-x divide-gray-200 rounded-lg shadow" role="alert">
        <i class="ri-information-line text-blue-600"></i>
        <div class="pl-4 text-sm font-normal">Top Right Position</div>
    </div>
</div>
```

## Example 5: Animated Toast Notifications

```html
<!-- Animated Success Toast -->
<div id="toast-animated-success" class="flex items-center w-full max-w-xs p-4 text-gray-500 bg-white rounded-lg shadow opacity-0 transform translate-y-4 transition-all duration-300" role="alert">
    <div class="inline-flex items-center justify-center flex-shrink-0 w-8 h-8 text-green-500 bg-green-100 rounded-lg">
        <i class="ri-check-line"></i>
    </div>
    <div class="ml-3 text-sm font-normal">Action completed successfully!</div>
    <button type="button" class="ml-auto -mx-1.5 -my-1.5 bg-white text-gray-400 hover:text-gray-900 rounded-lg p-1.5 hover:bg-gray-100 inline-flex h-8 w-8">
        <span class="sr-only">Close</span>
        <i class="ri-close-line w-5 h-5"></i>
    </button>
</div>

<!-- JavaScript for Animation -->
document.getElementById('show-animated-success').addEventListener('click', function() {
    const toast = document.getElementById('toast-animated-success');
    toast.classList.remove('opacity-0', 'translate-y-4');
    toast.classList.add('opacity-100', 'translate-y-0');
    
    setTimeout(() => {
        toast.classList.remove('opacity-100', 'translate-y-0');
        toast.classList.add('opacity-0', 'translate-y-4');
    }, 3000);
});
```
