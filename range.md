# Range Slider Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Range Slider
```html
<div>
    <label for="basic-range" class="block mb-2 text-sm font-medium text-gray-900">Default Range</label>
    <input id="basic-range" type="range" value="50" class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer">
</div>
```

## Example 2: Range Slider with Min/Max Values and Step
```html
<div>
    <label for="minmax-range" class="block mb-2 text-sm font-medium text-gray-900">Range with steps (min: 0, max: 10, step: 0.5)</label>
    <input id="minmax-range" type="range" min="0" max="10" step="0.5" value="5" class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer">
    <div class="flex justify-between mt-1 text-xs text-gray-500">
        <span>0</span>
        <span>2.5</span>
        <span>5.0</span>
        <span>7.5</span>
        <span>10</span>
    </div>
</div>
```

## Example 3: Range Slider with Value Display
```html
<div>
    <div class="flex justify-between items-center mb-2">
        <label for="value-range" class="text-sm font-medium text-gray-900">Volume</label>
        <div class="flex items-center">
            <i class="ri-volume-up-line text-gray-500 mr-2"></i>
            <span id="value-range-display" class="text-sm font-medium text-gray-900">50%</span>
        </div>
    </div>
    <input id="value-range" type="range" value="50" class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer" onInput="document.getElementById('value-range-display').textContent = this.value + '%'">
</div>
```

## Example 4: Styled Range Slider
```html
<div>
    <label for="styled-range" class="block mb-2 text-sm font-medium text-gray-900">Styled Range</label>
    <input id="styled-range" type="range" value="50" class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer accent-blue-600">
    <style>
        /* Custom Range Slider - Different browser compatibility */
        #styled-range::-webkit-slider-thumb {
            appearance: none;
            width: 18px;
            height: 18px;
            background: #3B82F6;
            border-radius: 50%;
            cursor: pointer;
        }
        #styled-range::-moz-range-thumb {
            width: 18px;
            height: 18px;
            background: #3B82F6;
            border-radius: 50%;
            cursor: pointer;
            border: none;
        }
    </style>
</div>
```

## Example 5: Range Slider with Color Options
```html
<div class="space-y-6">
    <div>
        <label for="red-range" class="block mb-2 text-sm font-medium text-gray-900">Red (R)</label>
        <input id="red-range" type="range" min="0" max="255" value="150" class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer accent-red-600">
    </div>
    <div>
        <label for="green-range" class="block mb-2 text-sm font-medium text-gray-900">Green (G)</label>
        <input id="green-range" type="range" min="0" max="255" value="150" class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer accent-green-600">
    </div>
    <div>
        <label for="blue-range" class="block mb-2 text-sm font-medium text-gray-900">Blue (B)</label>
        <input id="blue-range" type="range" min="0" max="255" value="150" class="w-full h-2 bg-gray-200 rounded-lg appearance-none cursor-pointer accent-blue-600">
    </div>
    <div class="flex items-center mt-4">
        <span class="text-sm font-medium text-gray-900 mr-3">Preview:</span>
        <div id="color-preview" class="w-12 h-12 rounded-lg border border-gray-300" style="background-color: rgb(150, 150, 150);"></div>
        <span id="color-value" class="ml-3 text-sm font-mono">#969696</span>
    </div>
</div>

<script>
    document.addEventListener('DOMContentLoaded', function() {
        const redRange = document.getElementById('red-range');
        const greenRange = document.getElementById('green-range');
        const blueRange = document.getElementById('blue-range');
        const colorPreview = document.getElementById('color-preview');
        const colorValue = document.getElementById('color-value');

        function updateColor() {
            const r = redRange.value;
            const g = greenRange.value;
            const b = blueRange.value;
            const rgbColor = `rgb(${r}, ${g}, ${b})`;
            const hexColor = `#${parseInt(r).toString(16).padStart(2, '0')}${parseInt(g).toString(16).padStart(2, '0')}${parseInt(b).toString(16).padStart(2, '0')}`;
            
            colorPreview.style.backgroundColor = rgbColor;
            colorValue.textContent = hexColor;
        }

        redRange.addEventListener('input', updateColor);
        greenRange.addEventListener('input', updateColor);
        blueRange.addEventListener('input', updateColor);
    });
</script>
```
