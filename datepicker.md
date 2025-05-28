# Datepicker Component Examples

## Example 1: Basic Datepicker
```html
<div class="relative max-w-sm">
    <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
        <i class="ri-calendar-line text-gray-500"></i>
    </div>
    <input 
        type="text" 
        id="basic-datepicker" 
        class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5"
        placeholder="Select date">
</div>

<script>
    flatpickr('#basic-datepicker', {
        dateFormat: 'Y-m-d',
        altInput: true,
        altFormat: 'F j, Y',
        animate: true
    });
</script>
```

## Example 2: Range Datepicker
```html
<div class="grid md:grid-cols-2 gap-4 max-w-lg">
    <div class="relative">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
            <i class="ri-calendar-event-line text-gray-500"></i>
        </div>
        <input 
            type="text" 
            id="range-start" 
            class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5"
            placeholder="Start date">
    </div>
    <div class="relative">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
            <i class="ri-calendar-check-line text-gray-500"></i>
        </div>
        <input 
            type="text" 
            id="range-end" 
            class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5"
            placeholder="End date">
    </div>
</div>

<script>
    flatpickr('#range-start', {
        dateFormat: 'Y-m-d',
        altInput: true,
        altFormat: 'F j, Y',
        animate: true,
        plugins: []
    });
    
    flatpickr('#range-end', {
        dateFormat: 'Y-m-d',
        altInput: true,
        altFormat: 'F j, Y',
        animate: true,
        plugins: []
    });
</script>
```

## Example 3: Themed Datepicker
```html
<!-- Primary Theme -->
<div class="bg-blue-50 border border-blue-200 p-4 rounded-lg">
    <label class="block mb-2 text-sm font-medium text-blue-700">Primary Theme</label>
    <div class="relative">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
            <i class="ri-calendar-line text-blue-500"></i>
        </div>
        <input 
            type="text" 
            id="primary-theme" 
            class="border border-blue-300 text-blue-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5 bg-white"
            placeholder="Select date">
    </div>
</div>

<script>
    flatpickr('#primary-theme', {
        dateFormat: 'Y-m-d',
        altInput: true,
        altFormat: 'F j, Y',
        theme: 'material_blue'
    });
</script>
```

## Example 4: Datepicker with Time
```html
<div class="relative">
    <label for="datetime-picker" class="block mb-2 text-sm font-medium text-gray-700">Appointment Date & Time</label>
    <div class="flex">
        <div class="relative flex-grow">
            <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
                <i class="ri-calendar-event-fill text-gray-500"></i>
            </div>
            <input 
                type="text" 
                id="datetime-picker" 
                class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5"
                placeholder="Select date and time">
        </div>
    </div>
</div>

<script>
    flatpickr('#datetime-picker', {
        enableTime: true,
        dateFormat: 'Y-m-d H:i',
        altInput: true,
        altFormat: 'F j, Y - h:i K',
        animate: true
    });
</script>
```

## Example 5: Advanced Datepicker Features
```html
<!-- Multiple Dates Selection -->
<div>
    <h3 class="text-lg font-medium text-gray-700 mb-3">Multiple Dates</h3>
    <div class="relative">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
            <i class="ri-calendar-line text-gray-500"></i>
        </div>
        <input 
            type="text" 
            id="multiple-dates" 
            class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5"
            placeholder="Select multiple dates">
        <p class="mt-1 text-xs text-gray-500">Click multiple dates to select them</p>
    </div>
</div>

<!-- Disabled Dates -->
<div>
    <h3 class="text-lg font-medium text-gray-700 mb-3">Disabled Dates</h3>
    <div class="relative">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
            <i class="ri-calendar-line text-gray-500"></i>
        </div>
        <input 
            type="text" 
            id="disabled-dates" 
            class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5"
            placeholder="Select date">
        <p class="mt-1 text-xs text-gray-500">Weekends are disabled</p>
    </div>
</div>

<script>
    // Multiple Dates
    flatpickr('#multiple-dates', {
        dateFormat: 'Y-m-d',
        altInput: true,
        altFormat: 'F j, Y',
        animate: true,
        mode: 'multiple'
    });
    
    // Disabled Dates
    flatpickr('#disabled-dates', {
        dateFormat: 'Y-m-d',
        altInput: true,
        altFormat: 'F j, Y',
        animate: true,
        disable: [
            function(date) {
                // Return true if it's a weekend
                return (date.getDay() === 0 || date.getDay() === 6);
            }
        ]
    });
</script>
```
