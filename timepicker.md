# Timepicker Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Timepicker
```html
<div class="relative max-w-sm">
    <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
        <i class="ri-time-line text-gray-500"></i>
    </div>
    <input type="time" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" required>
</div>
```

## Example 2: Timepicker with 12-hour format and label
```html
<div class="max-w-sm">
    <label for="time-picker-label" class="block mb-2 text-sm font-medium text-gray-900">Select an appointment time</label>
    <div class="relative">
        <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
            <i class="ri-calendar-event-line text-gray-500"></i>
        </div>
        <input type="time" id="time-picker-label" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" required>
    </div>
    <p class="mt-1 text-sm text-gray-500">Office hours are 9:00 AM to 5:00 PM</p>
</div>
```

## Example 3: Disabled Timepicker
```html
<div class="max-w-sm">
    <label for="disabled-time" class="block mb-2 text-sm font-medium text-gray-500">Closed Time (Disabled)</label>
    <div class="relative">
        <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
            <i class="ri-lock-line text-gray-400"></i>
        </div>
        <input type="time" id="disabled-time" class="bg-gray-100 border border-gray-300 text-gray-500 text-sm rounded-lg cursor-not-allowed block w-full ps-10 p-2.5" value="22:00" disabled>
    </div>
</div>
```

## Example 4: Timepicker with Validation
```html
<form class="max-w-sm">
    <div class="mb-4">
        <label for="time-valid" class="block mb-2 text-sm font-medium text-gray-900">Choose time (required)</label>
        <div class="relative">
            <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                <i class="ri-time-line text-gray-500"></i>
            </div>
            <input type="time" id="time-valid" class="bg-gray-50 border border-red-500 text-gray-900 text-sm rounded-lg focus:ring-red-500 focus:border-red-500 block w-full ps-10 p-2.5" required>
        </div>
        <p class="mt-2 text-sm text-red-600"><i class="ri-error-warning-line mr-1"></i>Please select a valid time.</p>
    </div>
    <button type="submit" class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center">Submit</button>
</form>
```

## Example 5: Timepicker Range (Start and End Time)
```html
<div class="max-w-sm space-y-4">
    <div>
        <label for="start-time" class="block mb-2 text-sm font-medium text-gray-900">Start Time</label>
        <div class="relative">
            <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                <i class="ri-play-circle-line text-gray-500"></i>
            </div>
            <input type="time" id="start-time" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" required>
        </div>
    </div>
    <div>
        <label for="end-time" class="block mb-2 text-sm font-medium text-gray-900">End Time</label>
        <div class="relative">
            <div class="absolute inset-y-0 start-0 flex items-center ps-3.5 pointer-events-none">
                <i class="ri-stop-circle-line text-gray-500"></i>
            </div>
            <input type="time" id="end-time" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full ps-10 p-2.5" required>
        </div>
    </div>
    <div class="flex justify-end">
        <button type="button" class="text-white bg-green-600 hover:bg-green-700 focus:ring-4 focus:outline-none focus:ring-green-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center flex items-center">
            <i class="ri-check-line mr-2"></i> Confirm Time Range
        </button>
    </div>
</div>
```
