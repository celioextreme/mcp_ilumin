# Progress Component Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Progress Bar

```html
<div class="mb-4">
    <div class="flex justify-between mb-1">
        <span class="text-base font-medium text-blue-700">Basic Progress</span>
        <span class="text-sm font-medium text-blue-700">75%</span>
    </div>
    <div class="w-full bg-gray-200 rounded-full h-2.5">
        <div class="bg-blue-600 h-2.5 rounded-full" style="width: 75%"></div>
    </div>
</div>

<div class="space-y-3 mt-8">
    <div class="flex justify-between mb-1">
        <span class="text-base font-medium text-red-700">Failed</span>
        <span class="text-sm font-medium text-red-700">25%</span>
    </div>
    <div class="w-full bg-gray-200 rounded-full h-2.5">
        <div class="bg-red-600 h-2.5 rounded-full" style="width: 25%"></div>
    </div>
    
    <div class="flex justify-between mb-1">
        <span class="text-base font-medium text-yellow-700">In Progress</span>
        <span class="text-sm font-medium text-yellow-700">50%</span>
    </div>
    <div class="w-full bg-gray-200 rounded-full h-2.5">
        <div class="bg-yellow-400 h-2.5 rounded-full" style="width: 50%"></div>
    </div>
    
    <div class="flex justify-between mb-1">
        <span class="text-base font-medium text-green-700">Success</span>
        <span class="text-sm font-medium text-green-700">100%</span>
    </div>
    <div class="w-full bg-gray-200 rounded-full h-2.5">
        <div class="bg-green-600 h-2.5 rounded-full" style="width: 100%"></div>
    </div>
</div>
```

## Example 2: Labeled Progress Bar

```html
<div class="mb-6">
    <h3 class="text-lg font-medium text-gray-900 mb-2">Project Status</h3>
    <div class="w-full bg-gray-200 rounded-full h-4">
        <div class="bg-blue-600 h-4 rounded-full text-xs font-medium text-blue-100 text-center p-0.5 leading-none" style="width: 65%">65%</div>
    </div>
</div>

<div class="space-y-6 mt-8">
    <div>
        <div class="flex justify-between mb-1">
            <span class="text-base font-medium text-gray-700">Design</span>
            <span class="text-sm font-medium text-gray-700">100%</span>
        </div>
        <div class="w-full bg-gray-200 rounded-full h-4">
            <div class="bg-green-600 h-4 rounded-full flex items-center justify-center text-xs font-medium text-white" style="width: 100%">
                <i class="ri-check-line mr-1"></i> Complete
            </div>
        </div>
    </div>
    
    <div>
        <div class="flex justify-between mb-1">
            <span class="text-base font-medium text-gray-700">Development</span>
            <span class="text-sm font-medium text-gray-700">65%</span>
        </div>
        <div class="w-full bg-gray-200 rounded-full h-4">
            <div class="bg-blue-600 h-4 rounded-full flex items-center justify-center text-xs font-medium text-white" style="width: 65%">
                <i class="ri-code-line mr-1"></i> In Progress
            </div>
        </div>
    </div>
    
    <div>
        <div class="flex justify-between mb-1">
            <span class="text-base font-medium text-gray-700">Testing</span>
            <span class="text-sm font-medium text-gray-700">25%</span>
        </div>
        <div class="w-full bg-gray-200 rounded-full h-4">
            <div class="bg-yellow-400 h-4 rounded-full flex items-center justify-center text-xs font-medium text-white" style="width: 25%">
                <i class="ri-bug-line mr-1"></i> Started
            </div>
        </div>
    </div>
</div>
```

## Example 3: Progress Bar with Steps

```html
<div class="mb-4">
    <h3 class="text-lg font-medium text-gray-900 mb-2">Checkout Progress</h3>
    <div class="w-full bg-gray-200 rounded-full h-2.5 mb-6">
        <div class="bg-blue-600 h-2.5 rounded-full" style="width: 50%"></div>
    </div>
    <div class="relative">
        <div class="flex justify-between mb-1">
            <div class="flex flex-col items-center">
                <div class="w-8 h-8 rounded-full bg-green-600 flex items-center justify-center text-white mb-1">
                    <i class="ri-check-line"></i>
                </div>
                <div class="text-xs text-center w-20">Cart</div>
            </div>
            <div class="flex flex-col items-center">
                <div class="w-8 h-8 rounded-full bg-green-600 flex items-center justify-center text-white mb-1">
                    <i class="ri-check-line"></i>
                </div>
                <div class="text-xs text-center w-20">Shipping</div>
            </div>
            <div class="flex flex-col items-center">
                <div class="w-8 h-8 rounded-full bg-blue-600 flex items-center justify-center text-white mb-1">
                    <i class="ri-user-line"></i>
                </div>
                <div class="text-xs text-center font-medium text-blue-600 w-20">Payment</div>
            </div>
            <div class="flex flex-col items-center">
                <div class="w-8 h-8 rounded-full bg-gray-400 flex items-center justify-center text-white mb-1">
                    <i class="ri-check-double-line"></i>
                </div>
                <div class="text-xs text-center text-gray-400 w-20">Confirmation</div>
            </div>
        </div>
    </div>
</div>
```

## Example 4: Circular Progress

```html
<div class="flex flex-wrap justify-center gap-8">
    <!-- SVG Circular Progress 75% -->
    <div class="flex flex-col items-center">
        <svg class="w-24 h-24" viewBox="0 0 36 36">
            <path class="stroke-current text-gray-200" stroke-width="3" fill="none" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
            <path class="stroke-current text-blue-600" stroke-width="3" fill="none" stroke-linecap="round" stroke-dasharray="75, 100" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
            <text x="18" y="20.5" text-anchor="middle" class="text-blue-600 font-medium text-3xl">75%</text>
        </svg>
        <div class="mt-2 text-center">
            <h4 class="font-medium">Downloads</h4>
            <p class="text-sm text-gray-600">1,500 / 2,000</p>
        </div>
    </div>
    
    <!-- Small Circle Progress Indicators -->
    <div class="flex flex-col items-center">
        <div class="relative">
            <svg class="w-14 h-14" viewBox="0 0 36 36">
                <path class="stroke-current text-gray-200" stroke-width="4" fill="none" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
                <path class="stroke-current text-purple-600" stroke-width="4" fill="none" stroke-linecap="round" stroke-dasharray="42, 100" d="M18 2.0845 a 15.9155 15.9155 0 0 1 0 31.831 a 15.9155 15.9155 0 0 1 0 -31.831"/>
            </svg>
            <div class="absolute inset-0 flex items-center justify-center">
                <i class="ri-user-line text-xl text-purple-600"></i>
            </div>
        </div>
        <div class="mt-2 text-center">
            <h4 class="text-sm font-medium">Profile</h4>
            <p class="text-xs text-gray-600">42%</p>
        </div>
    </div>
</div>
```

## Example 5: Animated Progress Bars

```html
<!-- Animated Bar with Stripes -->
<div class="mb-4">
    <div class="flex justify-between mb-1">
        <span class="text-base font-medium text-blue-700">Processing</span>
        <span class="text-sm font-medium text-blue-700">45%</span>
    </div>
    <div class="w-full bg-gray-200 rounded-full h-4">
        <div class="bg-gradient-to-r from-blue-500 to-blue-600 h-4 rounded-full relative overflow-hidden" style="width: 45%">
            <div class="absolute inset-0 animate-pulse opacity-25">
                <div class="absolute inset-0 bg-stripes" style="background-image: linear-gradient(45deg, rgba(255, 255, 255, 0.15) 25%, transparent 25%, transparent 50%, rgba(255, 255, 255, 0.15) 50%, rgba(255, 255, 255, 0.15) 75%, transparent 75%, transparent); background-size: 1rem 1rem;"></div>
            </div>
        </div>
    </div>
</div>

<!-- Gradient Progress Bar -->
<div class="mb-4">
    <div class="flex justify-between mb-1">
        <span class="text-base font-medium text-indigo-700">Score</span>
        <span class="text-sm font-medium text-indigo-700">82%</span>
    </div>
    <div class="w-full bg-gray-200 rounded-full h-4">
        <div class="bg-gradient-to-r from-indigo-500 via-purple-500 to-pink-500 h-4 rounded-full animate-gradient-x" style="width: 82%"></div>
    </div>
</div>

<!-- Loading Bar with Text -->
<div class="mb-4">
    <div class="w-full bg-gray-200 rounded-full h-6">
        <div class="bg-blue-600 h-6 rounded-full relative" style="width: 60%">
            <div class="absolute inset-0 flex items-center justify-center text-xs font-medium text-white">
                <i class="ri-loader-4-line animate-spin mr-1"></i>
                Loading Resources...
            </div>
        </div>
    </div>
</div>

<style>
@keyframes gradient-x {
    0% { background-position: 0% 50%; }
    50% { background-position: 100% 50%; }
    100% { background-position: 0% 50%; }
}
.animate-gradient-x {
    background-size: 200% 100%;
    animation: gradient-x 3s ease infinite;
}
</style>
```
