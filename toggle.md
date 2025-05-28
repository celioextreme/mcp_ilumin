# Toggle Switch Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Toggle Switch
```html
<label class="relative inline-flex items-center cursor-pointer">
    <input type="checkbox" value="" class="sr-only peer">
    <div class="w-11 h-6 bg-gray-200 peer-focus:outline-none peer-focus:ring-4 peer-focus:ring-blue-300 rounded-full peer peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all peer-checked:bg-blue-600"></div>
    <span class="ms-3 text-sm font-medium text-gray-900">Toggle me</span>
</label>
```

## Example 2: Toggle Switch with Icons
```html
<label class="relative inline-flex items-center cursor-pointer">
    <input type="checkbox" value="" class="sr-only peer">
    <div class="w-11 h-6 bg-gray-200 rounded-full peer peer-focus:ring-4 peer-focus:ring-green-300 peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all peer-checked:bg-green-600">
    </div>
    <span class="ms-3 text-sm font-medium text-gray-900 flex items-center">
        <i class="ri-sun-line text-lg mr-1 peer-checked:hidden"></i>
        <i class="ri-moon-line text-lg mr-1 hidden peer-checked:block"></i>
        <span class="peer-checked:hidden">Light</span>
        <span class="hidden peer-checked:block">Dark</span>
    </span>
</label>
```

## Example 3: Toggle Switch with Status Label
```html
<label class="relative inline-flex items-center cursor-pointer">
    <input type="checkbox" checked value="" class="sr-only peer">
    <div class="w-11 h-6 bg-gray-200 rounded-full peer peer-focus:ring-4 peer-focus:ring-blue-300 peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all peer-checked:bg-blue-600"></div>
    <span class="ms-3 text-sm font-medium text-gray-900">Active</span>
    <span class="ms-2 text-xs font-medium text-green-600">Online now</span>
</label>
```

## Example 4: Disabled Toggle Switches
```html
<div class="flex flex-col gap-4">
    <label class="relative inline-flex items-center">
        <input disabled type="checkbox" value="" class="sr-only peer">
        <div class="w-11 h-6 bg-gray-200 cursor-not-allowed opacity-70 rounded-full peer after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all"></div>
        <span class="ms-3 text-sm font-medium text-gray-400">Disabled</span>
    </label>
    
    <label class="relative inline-flex items-center">
        <input disabled checked type="checkbox" value="" class="sr-only peer">
        <div class="w-11 h-6 bg-blue-600 cursor-not-allowed opacity-70 rounded-full peer peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all"></div>
        <span class="ms-3 text-sm font-medium text-gray-400">Disabled checked</span>
    </label>
</div>
```

## Example 5: Toggle Switch Sizes
```html
<div class="flex flex-col gap-6">
    <label class="relative inline-flex items-center mb-3 cursor-pointer">
        <input type="checkbox" value="" class="sr-only peer">
        <div class="w-9 h-5 bg-gray-200 peer-focus:outline-none peer-focus:ring-4 peer-focus:ring-blue-300 rounded-full peer peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-4 after:w-4 after:transition-all peer-checked:bg-blue-600"></div>
        <span class="ms-3 text-sm font-medium text-gray-900">Small toggle</span>
    </label>
    
    <label class="relative inline-flex items-center mb-3 cursor-pointer">
        <input type="checkbox" value="" class="sr-only peer">
        <div class="w-11 h-6 bg-gray-200 peer-focus:outline-none peer-focus:ring-4 peer-focus:ring-blue-300 rounded-full peer peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-[2px] after:start-[2px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-5 after:w-5 after:transition-all peer-checked:bg-blue-600"></div>
        <span class="ms-3 text-sm font-medium text-gray-900">Default toggle</span>
    </label>
    
    <label class="relative inline-flex items-center mb-3 cursor-pointer">
        <input type="checkbox" value="" class="sr-only peer">
        <div class="w-14 h-7 bg-gray-200 peer-focus:outline-none peer-focus:ring-4 peer-focus:ring-blue-300 rounded-full peer peer-checked:after:translate-x-full rtl:peer-checked:after:-translate-x-full peer-checked:after:border-white after:content-[''] after:absolute after:top-0.5 after:start-[4px] after:bg-white after:border-gray-300 after:border after:rounded-full after:h-6 after:w-6 after:transition-all peer-checked:bg-blue-600"></div>
        <span class="ms-3 text-sm font-medium text-gray-900">Large toggle</span>
    </label>
</div>
```
