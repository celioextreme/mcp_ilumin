# Bottom Navigation Component Examples

## Example 1: Basic Bottom Navigation

```html
<div class="bg-white border-t border-gray-200 fixed bottom-0 left-0 right-0">
    <div class="grid grid-cols-5">
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-blue-500 border-t-2 border-blue-500">
            <i class="ri-home-line text-xl"></i>
            <span class="text-xs mt-1">Home</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-500 hover:text-blue-500">
            <i class="ri-search-line text-xl"></i>
            <span class="text-xs mt-1">Search</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-500 hover:text-blue-500">
            <i class="ri-add-circle-fill text-3xl -mt-5 text-blue-500"></i>
            <span class="text-xs mt-1">New</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-500 hover:text-blue-500">
            <i class="ri-heart-line text-xl"></i>
            <span class="text-xs mt-1">Favorites</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-500 hover:text-blue-500">
            <i class="ri-user-line text-xl"></i>
            <span class="text-xs mt-1">Profile</span>
        </button>
    </div>
</div>
```

## Example 2: Bottom Navigation with Notifications

```html
<div class="bg-white border-t border-gray-200 fixed bottom-0 left-0 right-0">
    <div class="grid grid-cols-4">
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-blue-500">
            <div class="relative">
                <i class="ri-home-line text-xl"></i>
            </div>
            <span class="text-xs mt-1">Home</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-500 hover:text-blue-500">
            <div class="relative">
                <i class="ri-chat-1-line text-xl"></i>
                <span class="absolute top-0 right-0 -mt-1 -mr-1 flex h-4 w-4 items-center justify-center rounded-full bg-red-500 text-xs text-white">3</span>
            </div>
            <span class="text-xs mt-1">Chats</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-500 hover:text-blue-500">
            <div class="relative">
                <i class="ri-notification-3-line text-xl"></i>
                <span class="absolute top-0 right-0 -mt-1 -mr-1 flex h-4 w-4 items-center justify-center rounded-full bg-red-500 text-xs text-white">5</span>
            </div>
            <span class="text-xs mt-1">Notifications</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-500 hover:text-blue-500">
            <div class="relative">
                <i class="ri-user-line text-xl"></i>
            </div>
            <span class="text-xs mt-1">Profile</span>
        </button>
    </div>
</div>
```

## Example 3: Dark Theme Bottom Navigation

```html
<div class="bg-gray-900 shadow-lg fixed bottom-0 left-0 right-0">
    <div class="grid grid-cols-5">
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-blue-400">
            <i class="ri-home-line text-xl"></i>
            <span class="text-xs mt-1">Home</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-400 hover:text-blue-400">
            <i class="ri-compass-line text-xl"></i>
            <span class="text-xs mt-1">Explore</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-400 hover:text-blue-400">
            <i class="ri-shopping-bag-line text-xl"></i>
            <span class="text-xs mt-1">Shop</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-400 hover:text-blue-400">
            <i class="ri-heart-line text-xl"></i>
            <span class="text-xs mt-1">Favorites</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center px-5 py-3 text-gray-400 hover:text-blue-400">
            <i class="ri-user-line text-xl"></i>
            <span class="text-xs mt-1">Profile</span>
        </button>
    </div>
</div>
```

## Example 4: Minimalist Bottom Navigation

```html
<div class="bg-white shadow-lg fixed bottom-0 left-0 right-0 p-2">
    <div class="flex justify-around">
        <button type="button" class="p-3 rounded-full text-blue-600 bg-blue-100">
            <i class="ri-home-line text-xl"></i>
        </button>
        <button type="button" class="p-3 rounded-full text-gray-500 hover:bg-gray-100">
            <i class="ri-search-line text-xl"></i>
        </button>
        <button type="button" class="p-3 rounded-full text-gray-500 hover:bg-gray-100">
            <i class="ri-heart-line text-xl"></i>
        </button>
        <button type="button" class="p-3 rounded-full text-gray-500 hover:bg-gray-100">
            <i class="ri-user-line text-xl"></i>
        </button>
    </div>
</div>
```

## Example 5: Bottom Navigation with Active Indicator

```html
<div class="bg-white border-t border-gray-200 fixed bottom-0 left-0 right-0 pb-1">
    <div class="relative flex justify-around">
        <!-- Active indicator dot -->
        <div class="absolute h-1 w-12 rounded-full bg-blue-500 -top-0.5 left-[12%] transition-all duration-300"></div>
        
        <button type="button" class="flex flex-col items-center justify-center pt-3 pb-1 w-full text-blue-500">
            <i class="ri-home-line text-xl"></i>
            <span class="text-xs font-medium mt-1">Home</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center pt-3 pb-1 w-full text-gray-400">
            <i class="ri-search-line text-xl"></i>
            <span class="text-xs mt-1">Search</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center pt-3 pb-1 w-full text-gray-400">
            <i class="ri-heart-line text-xl"></i>
            <span class="text-xs mt-1">Favorites</span>
        </button>
        <button type="button" class="flex flex-col items-center justify-center pt-3 pb-1 w-full text-gray-400">
            <i class="ri-user-line text-xl"></i>
            <span class="text-xs mt-1">Profile</span>
        </button>
    </div>
</div>
```
