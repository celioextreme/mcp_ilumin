# Badge Component Examples

## Example 1: Basic Badge Variants

```html
<div class="flex flex-wrap items-center gap-4">
    <!-- Default Badge -->
    <span class="bg-blue-100 text-blue-800 text-xs font-medium px-2.5 py-0.5 rounded">Default</span>
    
    <!-- Dark Badge -->
    <span class="bg-gray-100 text-gray-800 text-xs font-medium px-2.5 py-0.5 rounded">Dark</span>
    
    <!-- Red Badge -->
    <span class="bg-red-100 text-red-800 text-xs font-medium px-2.5 py-0.5 rounded">Red</span>
    
    <!-- Green Badge -->
    <span class="bg-green-100 text-green-800 text-xs font-medium px-2.5 py-0.5 rounded">Green</span>
    
    <!-- Yellow Badge -->
    <span class="bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded">Yellow</span>
    
    <!-- Indigo Badge -->
    <span class="bg-indigo-100 text-indigo-800 text-xs font-medium px-2.5 py-0.5 rounded">Indigo</span>
    
    <!-- Purple Badge -->
    <span class="bg-purple-100 text-purple-800 text-xs font-medium px-2.5 py-0.5 rounded">Purple</span>
    
    <!-- Pink Badge -->
    <span class="bg-pink-100 text-pink-800 text-xs font-medium px-2.5 py-0.5 rounded">Pink</span>
</div>
```

## Example 2: Pill Badges

```html
<div class="flex flex-wrap items-center gap-4">
    <!-- Blue Pill Badge -->
    <span class="bg-blue-100 text-blue-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Blue</span>
    
    <!-- Gray Pill Badge -->
    <span class="bg-gray-100 text-gray-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Gray</span>
    
    <!-- Red Pill Badge -->
    <span class="bg-red-100 text-red-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Red</span>
    
    <!-- Green Pill Badge -->
    <span class="bg-green-100 text-green-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Green</span>
    
    <!-- Yellow Pill Badge -->
    <span class="bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Yellow</span>
    
    <!-- Indigo Pill Badge -->
    <span class="bg-indigo-100 text-indigo-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Indigo</span>
    
    <!-- Purple Pill Badge -->
    <span class="bg-purple-100 text-purple-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Purple</span>
    
    <!-- Pink Pill Badge -->
    <span class="bg-pink-100 text-pink-800 text-xs font-medium px-2.5 py-0.5 rounded-full">Pink</span>
</div>
```

## Example 3: Badges with Icons

```html
<div class="flex flex-wrap items-center gap-4">
    <!-- Check Badge -->
    <span class="inline-flex items-center bg-green-100 text-green-800 text-xs font-medium px-2.5 py-0.5 rounded-full">
        <i class="ri-check-line mr-1"></i>
        Approved
    </span>
    
    <!-- Warning Badge -->
    <span class="inline-flex items-center bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded-full">
        <i class="ri-alert-line mr-1"></i>
        Warning
    </span>
    
    <!-- Error Badge -->
    <span class="inline-flex items-center bg-red-100 text-red-800 text-xs font-medium px-2.5 py-0.5 rounded-full">
        <i class="ri-close-circle-line mr-1"></i>
        Failed
    </span>
    
    <!-- Info Badge -->
    <span class="inline-flex items-center bg-blue-100 text-blue-800 text-xs font-medium px-2.5 py-0.5 rounded-full">
        <i class="ri-information-line mr-1"></i>
        Info
    </span>
    
    <!-- Lock Badge -->
    <span class="inline-flex items-center bg-gray-100 text-gray-800 text-xs font-medium px-2.5 py-0.5 rounded-full">
        <i class="ri-lock-line mr-1"></i>
        Locked
    </span>
</div>
```

## Example 4: Badge Size Variations

```html
<div class="flex flex-col space-y-4">
    <!-- Small Badge -->
    <div class="flex items-center gap-2">
        <span class="bg-blue-100 text-blue-800 text-xs font-medium px-2 py-0.5 rounded">Small</span>
        <span class="text-gray-500 text-sm">Default size for most use cases</span>
    </div>
    
    <!-- Medium Badge -->
    <div class="flex items-center gap-2">
        <span class="bg-blue-100 text-blue-800 text-sm font-medium px-2.5 py-0.5 rounded">Medium</span>
        <span class="text-gray-500 text-sm">Medium size for more visibility</span>
    </div>
    
    <!-- Large Badge -->
    <div class="flex items-center gap-2">
        <span class="bg-blue-100 text-blue-800 text-base font-medium px-3 py-1 rounded">Large</span>
        <span class="text-gray-500 text-sm">Large size for important information</span>
    </div>
    
    <!-- Extra Large Badge -->
    <div class="flex items-center gap-2">
        <span class="bg-blue-100 text-blue-800 text-lg font-medium px-3.5 py-1.5 rounded">Extra Large</span>
        <span class="text-gray-500 text-sm">Extra large size for high emphasis</span>
    </div>
</div>
```

## Example 5: Notification Badges

```html
<div class="flex flex-wrap items-center gap-8">
    <!-- Message Notification -->
    <div class="relative inline-flex">
        <button class="inline-flex items-center text-gray-700 bg-gray-100 hover:bg-gray-200 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5">
            <i class="ri-message-3-line text-lg mr-2"></i>
            Messages
        </button>
        <div class="absolute inline-flex items-center justify-center w-6 h-6 text-xs font-bold text-white bg-red-500 border-2 border-white rounded-full -top-2 -right-2">8</div>
    </div>
    
    <!-- Cart Notification -->
    <div class="relative inline-flex">
        <button class="inline-flex items-center text-gray-700 bg-gray-100 hover:bg-gray-200 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5">
            <i class="ri-shopping-cart-line text-lg mr-2"></i>
            Cart
        </button>
        <div class="absolute inline-flex items-center justify-center w-6 h-6 text-xs font-bold text-white bg-blue-500 border-2 border-white rounded-full -top-2 -right-2">4</div>
    </div>
    
    <!-- Notification Bell -->
    <div class="relative inline-flex">
        <button class="inline-flex items-center text-gray-700 bg-gray-100 hover:bg-gray-200 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-3 py-2.5">
            <i class="ri-notification-3-line text-xl"></i>
        </button>
        <div class="absolute inline-flex items-center justify-center w-5 h-5 text-xs font-bold text-white bg-red-500 border-2 border-white rounded-full -top-2 -right-2">3</div>
    </div>
    
    <!-- User Profile with Status -->
    <div class="relative inline-flex">
        <button class="inline-flex items-center text-gray-700 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-full text-sm p-1">
            <img class="w-10 h-10 rounded-full" src="https://i.pravatar.cc/100?img=3" alt="User profile">
        </button>
        <div class="absolute inline-flex items-center justify-center w-3 h-3 bg-green-500 border-2 border-white rounded-full bottom-0 right-0"></div>
    </div>
    
    <!-- Counter only notification -->
    <div class="relative inline-flex">
        <button class="inline-flex items-center text-gray-700 bg-gray-100 hover:bg-gray-200 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5">
            <i class="ri-mail-line text-lg mr-2"></i>
            Inbox
        </button>
        <span class="inline-flex items-center justify-center px-2 py-1 text-xs font-bold leading-none text-red-100 bg-red-600 rounded-full -top-2 -right-2 absolute">99+</span>
    </div>
</div>
```
