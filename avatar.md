# Avatar Component Examples

## Example 1: Basic Avatar Sizes

```html
<div class="flex flex-wrap items-center gap-6">
    <!-- Extra Small Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-6 h-6 rounded-full bg-indigo-500 flex items-center justify-center text-white text-xs overflow-hidden">
            <img src="https://i.pravatar.cc/100?img=1" alt="Avatar" class="w-full h-full object-cover">
        </div>
        <span class="text-xs text-gray-500 mt-1">XS</span>
    </div>
    
    <!-- Small Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-8 h-8 rounded-full bg-indigo-500 flex items-center justify-center text-white text-sm overflow-hidden">
            <img src="https://i.pravatar.cc/100?img=2" alt="Avatar" class="w-full h-full object-cover">
        </div>
        <span class="text-xs text-gray-500 mt-1">SM</span>
    </div>
    
    <!-- Medium Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-10 h-10 rounded-full bg-indigo-500 flex items-center justify-center text-white overflow-hidden">
            <img src="https://i.pravatar.cc/100?img=3" alt="Avatar" class="w-full h-full object-cover">
        </div>
        <span class="text-xs text-gray-500 mt-1">MD</span>
    </div>
    
    <!-- Large Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-indigo-500 flex items-center justify-center text-white text-xl overflow-hidden">
            <img src="https://i.pravatar.cc/100?img=4" alt="Avatar" class="w-full h-full object-cover">
        </div>
        <span class="text-xs text-gray-500 mt-1">LG</span>
    </div>
    
    <!-- Extra Large Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-16 h-16 rounded-full bg-indigo-500 flex items-center justify-center text-white text-2xl overflow-hidden">
            <img src="https://i.pravatar.cc/100?img=5" alt="Avatar" class="w-full h-full object-cover">
        </div>
        <span class="text-xs text-gray-500 mt-1">XL</span>
    </div>
</div>
```

## Example 2: Avatar With Status Indicator

```html
<div class="flex flex-wrap items-center gap-6">
    <!-- Online Status -->
    <div class="flex flex-col items-center">
        <div class="relative">
            <div class="w-12 h-12 rounded-full overflow-hidden">
                <img src="https://i.pravatar.cc/100?img=6" alt="Avatar" class="w-full h-full object-cover">
            </div>
            <div class="absolute bottom-0 right-0 w-3 h-3 bg-green-500 rounded-full border-2 border-white"></div>
        </div>
        <span class="text-xs text-gray-500 mt-1">Online</span>
    </div>
    
    <!-- Away Status -->
    <div class="flex flex-col items-center">
        <div class="relative">
            <div class="w-12 h-12 rounded-full overflow-hidden">
                <img src="https://i.pravatar.cc/100?img=7" alt="Avatar" class="w-full h-full object-cover">
            </div>
            <div class="absolute bottom-0 right-0 w-3 h-3 bg-yellow-500 rounded-full border-2 border-white"></div>
        </div>
        <span class="text-xs text-gray-500 mt-1">Away</span>
    </div>
    
    <!-- Busy Status -->
    <div class="flex flex-col items-center">
        <div class="relative">
            <div class="w-12 h-12 rounded-full overflow-hidden">
                <img src="https://i.pravatar.cc/100?img=8" alt="Avatar" class="w-full h-full object-cover">
            </div>
            <div class="absolute bottom-0 right-0 w-3 h-3 bg-red-500 rounded-full border-2 border-white"></div>
        </div>
        <span class="text-xs text-gray-500 mt-1">Busy</span>
    </div>
    
    <!-- Offline Status -->
    <div class="flex flex-col items-center">
        <div class="relative">
            <div class="w-12 h-12 rounded-full overflow-hidden">
                <img src="https://i.pravatar.cc/100?img=9" alt="Avatar" class="w-full h-full object-cover">
            </div>
            <div class="absolute bottom-0 right-0 w-3 h-3 bg-gray-400 rounded-full border-2 border-white"></div>
        </div>
        <span class="text-xs text-gray-500 mt-1">Offline</span>
    </div>
</div>
```

## Example 3: Avatar With Text Fallback

```html
<div class="flex flex-wrap items-center gap-6">
    <!-- Avatar with initials -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-indigo-500 flex items-center justify-center text-white text-lg font-semibold">
            JD
        </div>
        <span class="text-xs text-gray-500 mt-1">John Doe</span>
    </div>
    
    <!-- Avatar with initials - different color -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-emerald-500 flex items-center justify-center text-white text-lg font-semibold">
            AS
        </div>
        <span class="text-xs text-gray-500 mt-1">Anna Smith</span>
    </div>
    
    <!-- Avatar with initials - different color -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-amber-500 flex items-center justify-center text-white text-lg font-semibold">
            RJ
        </div>
        <span class="text-xs text-gray-500 mt-1">Robert Johnson</span>
    </div>
    
    <!-- Avatar with initials - different color -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-rose-500 flex items-center justify-center text-white text-lg font-semibold">
            EW
        </div>
        <span class="text-xs text-gray-500 mt-1">Emma Wilson</span>
    </div>
</div>
```

## Example 4: Avatar Group

```html
<div class="flex -space-x-3">
    <img class="w-10 h-10 rounded-full border-2 border-white" src="https://i.pravatar.cc/100?img=10" alt="">
    <img class="w-10 h-10 rounded-full border-2 border-white" src="https://i.pravatar.cc/100?img=11" alt="">
    <img class="w-10 h-10 rounded-full border-2 border-white" src="https://i.pravatar.cc/100?img=12" alt="">
    <img class="w-10 h-10 rounded-full border-2 border-white" src="https://i.pravatar.cc/100?img=13" alt="">
    <div class="flex items-center justify-center w-10 h-10 rounded-full border-2 border-white bg-gray-700 text-xs font-medium text-white">
        +8
    </div>
</div>
```

## Example 5: Avatar With Remix Icons

```html
<div class="flex flex-wrap items-center gap-6">
    <!-- User Icon Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-blue-500 flex items-center justify-center text-white">
            <i class="ri-user-fill text-xl"></i>
        </div>
        <span class="text-xs text-gray-500 mt-1">User</span>
    </div>
    
    <!-- Admin Icon Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-purple-500 flex items-center justify-center text-white">
            <i class="ri-admin-fill text-xl"></i>
        </div>
        <span class="text-xs text-gray-500 mt-1">Admin</span>
    </div>
    
    <!-- Customer Support Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-green-500 flex items-center justify-center text-white">
            <i class="ri-customer-service-fill text-xl"></i>
        </div>
        <span class="text-xs text-gray-500 mt-1">Support</span>
    </div>
    
    <!-- Guest Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-orange-500 flex items-center justify-center text-white">
            <i class="ri-user-unfollow-fill text-xl"></i>
        </div>
        <span class="text-xs text-gray-500 mt-1">Guest</span>
    </div>
    
    <!-- Bot Avatar -->
    <div class="flex flex-col items-center">
        <div class="w-12 h-12 rounded-full bg-cyan-500 flex items-center justify-center text-white">
            <i class="ri-robot-fill text-xl"></i>
        </div>
        <span class="text-xs text-gray-500 mt-1">Bot</span>
    </div>
</div>
```
