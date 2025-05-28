# Headings Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Headings (h1-h6)
```html
<h1 class="text-5xl font-bold">This is H1 Heading</h1>
<h2 class="text-4xl font-bold">This is H2 Heading</h2>
<h3 class="text-3xl font-bold">This is H3 Heading</h3>
<h4 class="text-2xl font-bold">This is H4 Heading</h4>
<h5 class="text-xl font-bold">This is H5 Heading</h5>
<h6 class="text-lg font-bold">This is H6 Heading</h6>
```

## Example 2: Headings with Different Styles
```html
<h3 class="text-3xl font-light text-gray-800">Light Heading</h3>
<h3 class="text-3xl font-normal text-gray-800">Normal Heading</h3>
<h3 class="text-3xl font-medium text-gray-800">Medium Heading</h3>
<h3 class="text-3xl font-semibold text-gray-800">Semi-bold Heading</h3>
<h3 class="text-3xl font-bold text-gray-800">Bold Heading</h3>
<h3 class="text-3xl font-extrabold text-gray-800">Extra Bold Heading</h3>
```

## Example 3: Headings with Colors and Underlines
```html
<h3 class="text-3xl font-bold text-blue-600">Blue Heading</h3>

<h3 class="text-3xl font-bold text-green-600">Green Heading</h3>

<div>
    <h3 class="text-3xl font-bold text-purple-600 pb-2 border-b-4 border-purple-600 inline-block">
        Underlined Heading
    </h3>
</div>

<div>
    <h3 class="text-3xl font-bold text-gray-800 relative pb-2">
        <span class="bg-gradient-to-r from-blue-600 to-purple-600 bg-clip-text text-transparent">
            Gradient Text Heading
        </span>
    </h3>
</div>

<div>
    <h3 class="text-3xl font-bold text-white p-4 bg-gradient-to-r from-blue-500 to-purple-500 rounded-lg">
        Heading with Background
    </h3>
</div>
```

## Example 4: Headings with Icons and Badges
```html
<div class="flex items-center">
    <i class="ri-star-fill text-yellow-500 text-3xl mr-2"></i>
    <h3 class="text-3xl font-bold text-gray-800">Heading with Icon</h3>
</div>

<div class="flex items-center">
    <h3 class="text-3xl font-bold text-gray-800">Heading with Badge</h3>
    <span class="bg-blue-100 text-blue-800 text-sm font-medium me-2 px-2.5 py-0.5 rounded ms-3">New</span>
</div>

<div class="flex items-center flex-wrap">
    <h3 class="text-3xl font-bold text-gray-800 mr-3">Product Features</h3>
    <div class="flex flex-wrap gap-2">
        <span class="bg-blue-100 text-blue-800 text-xs font-medium px-2.5 py-0.5 rounded">Design</span>
        <span class="bg-green-100 text-green-800 text-xs font-medium px-2.5 py-0.5 rounded">Quality</span>
        <span class="bg-yellow-100 text-yellow-800 text-xs font-medium px-2.5 py-0.5 rounded">Performance</span>
    </div>
</div>

<div>
    <h3 class="text-3xl font-bold text-gray-800 flex items-center">
        <i class="ri-notification-fill text-red-500 mr-2"></i> 
        Important Update 
        <span class="bg-red-100 text-red-800 text-xs font-medium px-2.5 py-0.5 rounded ml-3">Urgent</span>
    </h3>
</div>
```

## Example 5: Responsive Headings and Special Layouts
```html
<h3 class="text-xl md:text-2xl lg:text-4xl font-bold text-gray-800">Responsive Heading</h3>
<p class="text-sm text-gray-500">This heading changes size based on screen width</p>

<div class="relative">
    <div class="absolute inset-0 flex items-center">
        <div class="border-t border-gray-300 w-full"></div>
    </div>
    <div class="relative flex justify-center">
        <span class="bg-white px-4 text-2xl font-bold text-gray-800">
            Centered with Lines
        </span>
    </div>
</div>

<div class="border-l-4 border-blue-500 pl-4">
    <h3 class="text-2xl font-bold text-gray-800">Left Border Accent</h3>
    <p class="text-gray-600">Subtitle or additional information</p>
</div>

<div class="bg-gray-50 p-6 rounded-lg">
    <div class="flex items-center justify-between">
        <h3 class="text-2xl font-bold text-gray-800">Card-style Heading</h3>
        <button class="text-blue-600 hover:text-blue-800">
            <i class="ri-more-2-fill text-xl"></i>
        </button>
    </div>
    <p class="text-gray-600 mt-1">With action buttons and container</p>
</div>
```
