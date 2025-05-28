# Horizontal Rule (HR) Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Horizontal Rule
```html
<p class="text-gray-700 mb-4">This is a paragraph of text followed by a basic horizontal rule that spans the full width of its container.</p>
<hr class="h-px my-8 bg-gray-200 border-0">
<p class="text-gray-700 mt-4">This is another paragraph of text after the horizontal rule.</p>
```

## Example 2: Styled HR with Custom Height and Color
```html
<p class="text-gray-700 mb-4">Here are examples of horizontal rules with different heights and colors.</p>

<hr class="h-0.5 my-6 bg-blue-500 border-0">
<p class="text-sm text-gray-500 mb-6">Height: 0.125rem (h-0.5), Color: Blue</p>

<hr class="h-1 my-6 bg-red-500 border-0">
<p class="text-sm text-gray-500 mb-6">Height: 0.25rem (h-1), Color: Red</p>

<hr class="h-2 my-6 bg-green-500 border-0">
<p class="text-sm text-gray-500">Height: 0.5rem (h-2), Color: Green</p>
```

## Example 3: HR with Text Label
```html
<p class="text-gray-700 mb-4">A horizontal rule with a text label in the middle, useful for section breaks.</p>

<div class="relative flex items-center py-5">
    <div class="flex-grow border-t border-gray-300"></div>
    <span class="flex-shrink px-4 text-gray-600">Section Divider</span>
    <div class="flex-grow border-t border-gray-300"></div>
</div>

<p class="text-gray-700 mb-4">Another variation with an icon.</p>

<div class="relative flex items-center py-5">
    <div class="flex-grow border-t border-gray-300"></div>
    <span class="flex-shrink mx-4 flex items-center text-gray-600">
        <i class="ri-star-line mr-2"></i> Featured Content
    </span>
    <div class="flex-grow border-t border-gray-300"></div>
</div>
```

## Example 4: Gradient and Styled HRs
```html
<p class="text-gray-700 mb-4">Horizontal rules with gradient effects for more visual appeal.</p>

<hr class="h-1 my-8 bg-gradient-to-r from-blue-500 via-purple-500 to-pink-500 border-0">
<p class="text-sm text-gray-500 mb-6">Gradient HR: Blue to Purple to Pink</p>

<hr class="h-1 my-8 bg-gradient-to-r from-green-300 to-blue-500 border-0">
<p class="text-sm text-gray-500 mb-6">Gradient HR: Green to Blue</p>

<div class="flex items-center my-8">
    <div class="flex-grow h-0.5 bg-gray-300"></div>
    <div class="mx-2 bg-blue-500 rounded-full w-2 h-2"></div>
    <div class="mx-2 bg-blue-500 rounded-full w-2 h-2"></div>
    <div class="mx-2 bg-blue-500 rounded-full w-2 h-2"></div>
    <div class="flex-grow h-0.5 bg-gray-300"></div>
</div>
<p class="text-sm text-gray-500">Styled HR with Dots</p>
```

## Example 5: Decorative and Themed HRs
```html
<p class="text-gray-700 mb-4">More creative horizontal rules for different design themes.</p>

<!-- Zigzag HR -->
<div class="my-8 flex justify-center">
    <svg width="100%" height="20" fill="none" xmlns="http://www.w3.org/2000/svg">
        <path d="M0 9H30L45 1L60 17L75 1L90 17L105 1L120 17L135 1L150 17L165 1L180 17L195 1L210 17L225 1L240 17L255 1L270 17L285 1L300 17L315 1L330 17L345 1L360 17L375 1L390 17L405 1L420 17L435 1L450 17L465 1L480 17L495 1L510 17L525 1L540 17L555 1L570 17L585 1L600 17L615 1L630 17L645 1L660 17L675 1L690 17L705 1L720 17L735 1L750 17L765 1L780 17L795 1L810 17L825 1L840 17L855 1L870 17L885 1L900 17L915 1L930 17L945 1L960 17L975 1L990 17L1005 1L1020 17L1035 1L1050 17L1065 1L1080 17L1095 1L1110 17L1125 1L1140 17L1155 1L1170 17L1185 1L1200 17" stroke="#CBD5E0" stroke-width="2"/>
    </svg>
</div>
<p class="text-sm text-gray-500 mb-6">Zigzag Pattern HR</p>

<!-- Dashed HR -->
<hr class="border-0 border-t-2 border-dashed border-gray-300 my-8">
<p class="text-sm text-gray-500 mb-6">Dashed Border HR</p>

<!-- Dotted HR -->
<hr class="border-0 border-t-2 border-dotted border-gray-300 my-8">
<p class="text-sm text-gray-500 mb-6">Dotted Border HR</p>

<!-- Shadow HR -->
<div class="my-8 h-px bg-gray-300 relative">
    <div class="absolute inset-0 bg-gradient-to-b from-transparent via-gray-500 to-transparent opacity-20"></div>
</div>
<p class="text-sm text-gray-500">Shadow Effect HR</p>
```
