# Indicators Component Examples

## Example 1: Basic Status Indicators
```html
<div class="p-4 bg-gray-50 rounded-lg space-y-6">
    <div class="flex items-center space-x-4">
        <div class="flex items-center">
            <span class="w-3 h-3 bg-green-500 rounded-full mr-2"></span>
            <span class="text-sm text-gray-700">Online</span>
        </div>
        <div class="flex items-center">
            <span class="w-3 h-3 bg-red-500 rounded-full mr-2"></span>
            <span class="text-sm text-gray-700">Offline</span>
        </div>
        <div class="flex items-center">
            <span class="w-3 h-3 bg-yellow-500 rounded-full mr-2"></span>
            <span class="text-sm text-gray-700">Away</span>
        </div>
        <div class="flex items-center">
            <span class="w-3 h-3 bg-gray-400 rounded-full mr-2"></span>
            <span class="text-sm text-gray-700">Inactive</span>
        </div>
    </div>
    <div class="flex items-center space-x-6">
        <div class="flex items-center space-x-3">
            <div class="relative">
                <img class="w-10 h-10 rounded-full" src="https://randomuser.me/api/portraits/women/12.jpg" alt="User Avatar">
                <span class="absolute bottom-0 right-0 w-3 h-3 bg-green-500 border-2 border-white rounded-full"></span>
            </div>
            <span class="text-sm font-medium text-gray-700">Emma Smith</span>
        </div>
    </div>
</div>
```

## Example 2: Animated Status Indicators
```html
<div class="p-4 bg-gray-50 rounded-lg space-y-6">
    <div class="flex items-center space-x-6">
        <!-- Pulsing Green Status -->
        <div class="flex items-center">
            <span class="relative flex h-3 w-3 mr-2">
                <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-green-400 opacity-75"></span>
                <span class="relative inline-flex rounded-full h-3 w-3 bg-green-500"></span>
            </span>
            <span class="text-sm text-gray-700">Live</span>
        </div>

        <!-- Pulsing Red Status -->
        <div class="flex items-center">
            <span class="relative flex h-3 w-3 mr-2">
                <span class="animate-ping absolute inline-flex h-full w-full rounded-full bg-red-400 opacity-75"></span>
                <span class="relative inline-flex rounded-full h-3 w-3 bg-red-500"></span>
            </span>
            <span class="text-sm text-gray-700">Recording</span>
        </div>

        <!-- Loading Indicator -->
        <div class="flex items-center">
            <svg class="animate-spin h-4 w-4 text-blue-500 mr-2" xmlns="http://www.w3.org/2000/svg" fill="none" viewBox="0 0 24 24">
                <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
            </svg>
            <span class="text-sm text-gray-700">Loading</span>
        </div>
    </div>
</div>
```

## Example 3: Notification Indicators
```html
<div class="p-4 bg-gray-50 rounded-lg">
    <div class="flex flex-wrap gap-8">
        <!-- Notification Bell -->
        <div class="flex items-center">
            <div class="relative">
                <button class="p-2 bg-white rounded-full shadow-sm border border-gray-200 text-gray-500 hover:bg-gray-50">
                    <i class="ri-notification-3-line text-xl"></i>
                </button>
                <span class="absolute top-0 right-0 inline-flex items-center justify-center px-2 py-1 text-xs font-bold leading-none text-white transform translate-x-1/2 -translate-y-1/2 bg-red-500 rounded-full">3</span>
            </div>
        </div>

        <!-- Message Icon -->
        <div class="flex items-center">
            <div class="relative">
                <button class="p-2 bg-white rounded-full shadow-sm border border-gray-200 text-gray-500 hover:bg-gray-50">
                    <i class="ri-message-2-line text-xl"></i>
                </button>
                <span class="absolute top-0 right-0 inline-flex items-center justify-center w-5 h-5 text-xs font-bold leading-none text-white transform translate-x-1/2 -translate-y-1/2 bg-blue-500 rounded-full">7</span>
            </div>
        </div>
    </div>
</div>
```

## Example 4: Progress Indicators
```html
<div class="p-4 bg-gray-50 rounded-lg space-y-8">
    <!-- File Upload Progress -->
    <div class="p-4 bg-white rounded-lg border border-gray-200 shadow-sm">
        <div class="flex justify-between mb-2">
            <div>
                <p class="text-sm font-medium text-gray-800">Uploading presentation.pdf</p>
                <p class="text-xs text-gray-500">3.2 MB of 8.5 MB</p>
            </div>
            <span class="text-sm text-gray-700">38%</span>
        </div>
        <div class="w-full h-2 bg-gray-200 rounded-full">
            <div class="h-2 bg-blue-500 rounded-full" style="width: 38%"></div>
        </div>
    </div>

    <!-- Step Progress -->
    <div class="space-y-4">
        <div class="flex items-center space-x-2">
            <div class="w-8 h-8 bg-green-500 text-white rounded-full flex items-center justify-center">
                <i class="ri-check-line"></i>
            </div>
            <div class="h-0.5 flex-1 bg-green-500"></div>
            <div class="w-8 h-8 bg-blue-500 text-white rounded-full flex items-center justify-center">2</div>
            <div class="h-0.5 flex-1 bg-gray-300"></div>
            <div class="w-8 h-8 bg-gray-200 text-gray-500 rounded-full flex items-center justify-center">3</div>
        </div>
    </div>
</div>
```

## Example 5: Status and State Indicators
```html
<div class="p-4 bg-gray-50 rounded-lg space-y-6">
    <!-- Status Pills -->
    <div class="flex flex-wrap gap-3">
        <span class="px-3 py-1 text-xs font-medium rounded-full bg-green-100 text-green-800">Approved</span>
        <span class="px-3 py-1 text-xs font-medium rounded-full bg-yellow-100 text-yellow-800">Pending</span>
        <span class="px-3 py-1 text-xs font-medium rounded-full bg-red-100 text-red-800">Rejected</span>
        <span class="px-3 py-1 text-xs font-medium rounded-full bg-blue-100 text-blue-800">In Progress</span>
    </div>

    <!-- Status with Icon -->
    <div class="flex flex-wrap gap-3">
        <div class="inline-flex items-center px-3 py-1 bg-green-100 text-green-800 rounded-full">
            <i class="ri-check-line mr-1"></i>
            <span class="text-xs font-medium">Verified</span>
        </div>
        <div class="inline-flex items-center px-3 py-1 bg-red-100 text-red-800 rounded-full">
            <i class="ri-error-warning-line mr-1"></i>
            <span class="text-xs font-medium">Failed</span>
        </div>
    </div>
    
    <!-- Status Tracking -->
    <div class="p-4 bg-white border border-gray-200 rounded-lg shadow-sm">
        <h3 class="text-sm font-medium text-gray-800 mb-3">Order #38492</h3>
        <div class="flex items-start space-x-2">
            <div class="flex flex-col items-center">
                <div class="w-6 h-6 rounded-full bg-green-500 text-white flex items-center justify-center text-xs">
                    <i class="ri-check-line"></i>
                </div>
                <div class="w-1 h-8 bg-green-500"></div>
            </div>
            <div>
                <p class="text-sm font-medium text-gray-800">Order Placed</p>
                <p class="text-xs text-gray-500">May 22, 2025 - 10:30 AM</p>
            </div>
        </div>
    </div>
</div>
```
