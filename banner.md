# Banner Component Examples

## Example 1: Simple Information Banner

```html
<!-- Information Banner -->
<div class="flex p-4 mb-4 text-sm text-blue-800 border border-blue-300 rounded-lg bg-blue-50">
    <i class="ri-information-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Info alert!</span> Change a few things up and try submitting again.
    </div>
</div>

<!-- Warning Banner -->
<div class="flex p-4 mb-4 text-sm text-yellow-800 border border-yellow-300 rounded-lg bg-yellow-50">
    <i class="ri-alert-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Warning alert!</span> Please review your information before proceeding.
    </div>
</div>

<!-- Error Banner -->
<div class="flex p-4 mb-4 text-sm text-red-800 border border-red-300 rounded-lg bg-red-50">
    <i class="ri-error-warning-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Error alert!</span> Something went wrong. Please try again later.
    </div>
</div>

<!-- Success Banner -->
<div class="flex p-4 text-sm text-green-800 border border-green-300 rounded-lg bg-green-50">
    <i class="ri-checkbox-circle-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Success alert!</span> Your changes have been saved successfully.
    </div>
</div>
```

## Example 2: Banner with Dismiss Button

```html
<!-- Information Banner with Dismiss -->
<div id="info-banner" class="flex items-center p-4 mb-4 text-sm text-blue-800 border border-blue-300 rounded-lg bg-blue-50">
    <i class="ri-information-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div class="flex-1">
        <span class="font-medium">Info alert!</span> Change a few things up and try submitting again.
    </div>
    <button type="button" onclick="document.getElementById('info-banner').style.display = 'none'" class="ml-auto -mx-1.5 -my-1.5 bg-blue-50 text-blue-500 rounded-lg focus:ring-2 focus:ring-blue-400 p-1.5 hover:bg-blue-200 inline-flex items-center justify-center h-8 w-8">
        <i class="ri-close-line"></i>
        <span class="sr-only">Close</span>
    </button>
</div>

<!-- Warning Banner with Dismiss -->
<div id="warning-banner" class="flex items-center p-4 mb-4 text-sm text-yellow-800 border border-yellow-300 rounded-lg bg-yellow-50">
    <i class="ri-alert-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div class="flex-1">
        <span class="font-medium">Warning alert!</span> Please review your information before proceeding.
    </div>
    <button type="button" onclick="document.getElementById('warning-banner').style.display = 'none'" class="ml-auto -mx-1.5 -my-1.5 bg-yellow-50 text-yellow-500 rounded-lg focus:ring-2 focus:ring-yellow-400 p-1.5 hover:bg-yellow-200 inline-flex items-center justify-center h-8 w-8">
        <i class="ri-close-line"></i>
        <span class="sr-only">Close</span>
    </button>
</div>
```

## Example 3: Solid Background Banners

```html
<!-- Solid Info Banner -->
<div class="flex items-center p-4 mb-4 text-white bg-blue-600 rounded-lg">
    <i class="ri-information-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Info alert!</span> Change a few things up and try submitting again.
    </div>
</div>

<!-- Solid Warning Banner -->
<div class="flex items-center p-4 mb-4 text-white bg-yellow-600 rounded-lg">
    <i class="ri-alert-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Warning alert!</span> Please review your information before proceeding.
    </div>
</div>

<!-- Solid Error Banner -->
<div class="flex items-center p-4 mb-4 text-white bg-red-600 rounded-lg">
    <i class="ri-error-warning-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Error alert!</span> Something went wrong. Please try again later.
    </div>
</div>

<!-- Solid Success Banner -->
<div class="flex items-center p-4 text-white bg-green-600 rounded-lg">
    <i class="ri-checkbox-circle-line flex-shrink-0 inline w-5 h-5 mr-3"></i>
    <div>
        <span class="font-medium">Success alert!</span> Your changes have been saved successfully.
    </div>
</div>
```

## Example 4: Banner with Actions

```html
<!-- Banner with Actions -->
<div class="flex flex-col md:flex-row p-4 mb-4 bg-yellow-100 border border-yellow-300 rounded-lg">
    <div class="flex items-center mb-2 md:mb-0">
        <i class="ri-alert-line flex-shrink-0 inline w-5 h-5 mr-3 text-yellow-700"></i>
        <div class="text-sm text-yellow-700">
            <span class="font-medium">Your trial is ending soon!</span> You have 3 days left in your trial period.
        </div>
    </div>
    <div class="ml-auto mt-2 md:mt-0 flex flex-col sm:flex-row gap-2">
        <button type="button" class="py-1.5 px-3 text-xs font-medium text-center text-white bg-yellow-700 hover:bg-yellow-800 rounded-lg focus:ring-2 focus:ring-yellow-300">Upgrade to Pro</button>
        <button type="button" class="py-1.5 px-3 text-xs font-medium text-center text-yellow-700 border border-yellow-700 hover:bg-yellow-200 rounded-lg focus:ring-2 focus:ring-yellow-300">Remind me later</button>
    </div>
</div>

<!-- Cookie Notice Banner -->
<div class="flex flex-col md:flex-row p-4 bg-gray-100 border border-gray-300 rounded-lg">
    <div class="flex items-center mb-2 md:mb-0">
        <i class="ri-cookie-line flex-shrink-0 inline w-5 h-5 mr-3 text-gray-700"></i>
        <div class="text-sm text-gray-700">
            <span class="font-medium">Cookie Notice</span> We use cookies to ensure you get the best experience on our website.
        </div>
    </div>
    <div class="ml-auto mt-2 md:mt-0 flex flex-col sm:flex-row gap-2">
        <button type="button" class="py-1.5 px-3 text-xs font-medium text-center text-white bg-blue-600 hover:bg-blue-700 rounded-lg focus:ring-2 focus:ring-blue-300">Accept All</button>
        <button type="button" class="py-1.5 px-3 text-xs font-medium text-center text-gray-700 border border-gray-700 hover:bg-gray-200 rounded-lg focus:ring-2 focus:ring-gray-300">Customize</button>
    </div>
</div>
```

## Example 5: Full-Width Top Banner

```html
<!-- Top Banner - Promotional -->
<div class="bg-gradient-to-r from-purple-600 to-indigo-600 py-3 px-4 mb-6 -mx-6 -mt-6 rounded-t-lg">
    <div class="flex flex-col sm:flex-row items-center justify-center">
        <div class="flex items-center text-white mb-2 sm:mb-0">
            <i class="ri-gift-line mr-2"></i>
            <p class="text-sm font-medium">Special offer: Get 30% off your first month with code <span class="font-bold">WELCOME30</span></p>
        </div>
        <button class="ml-0 sm:ml-4 px-4 py-1 text-xs font-medium text-purple-900 bg-white rounded-full hover:bg-gray-200 focus:ring-2 focus:ring-white">
            Claim Now
        </button>
    </div>
</div>

<!-- Top Banner - Announcement -->
<div class="bg-blue-800 py-3 px-4 mb-6 -mx-6 -mt-6 rounded-t-lg">
    <div class="flex items-center justify-between">
        <div class="flex items-center text-white">
            <i class="ri-megaphone-line mr-2"></i>
            <p class="text-sm font-medium">System maintenance scheduled for June 1, 2025. <a href="#" class="underline hover:text-blue-200">Learn more</a></p>
        </div>
        <button id="close-top-banner" onclick="this.parentElement.parentElement.style.display = 'none';" class="text-white hover:text-blue-200">
            <i class="ri-close-line text-lg"></i>
            <span class="sr-only">Close</span>
        </button>
    </div>
</div>
```
