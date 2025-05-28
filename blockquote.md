# Tailwind CSS Blockquote Examples

## Example 1: Simple Elegant Blockquote

```html
<blockquote class="pl-4 border-l-4 border-blue-500 italic text-gray-700">
    <p class="mb-2">"The best way to predict the future is to invent it. The future is not laid out on a track. It is something that we can decide, and to the extent that we do not violate any known laws of the universe, we can probably make it work the way that we want to."</p>
    <footer class="text-sm text-gray-600 mt-1 not-italic">
        — Alan Kay
    </footer>
</blockquote>
```

## Example 2: Modern Blockquote with Quote Icons

```html
<blockquote class="relative p-6 bg-gray-50 rounded-lg">
    <i class="ri-double-quotes-l text-4xl absolute top-2 left-2 text-gray-300"></i>
    <i class="ri-double-quotes-r text-4xl absolute bottom-2 right-2 text-gray-300"></i>
    <div class="relative z-10">
        <p class="text-lg text-gray-700 leading-relaxed">
            Design is not just what it looks like and feels like. Design is how it works. The details are not the details. They make the design. Simplicity is not the absence of clutter, that's a consequence of simplicity. Simplicity is somehow essentially describing the purpose and place of an object and product.
        </p>
        <footer class="mt-4 flex items-center">
            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="Steve Jobs" class="w-10 h-10 rounded-full mr-3">
            <div>
                <cite class="font-medium text-gray-900 not-italic">Steve Jobs</cite>
                <p class="text-sm text-gray-600">Co-founder of Apple Inc.</p>
            </div>
        </footer>
    </div>
</blockquote>
```

## Example 3: Colorful Card Blockquote

```html
<div class="rounded-lg overflow-hidden">
    <div class="bg-gradient-to-r from-purple-600 to-indigo-600 py-4 px-6 text-white">
        <i class="ri-double-quotes-l text-white text-opacity-30 text-3xl"></i>
    </div>
    <blockquote class="bg-white px-6 py-8 shadow-lg border-t-0">
        <p class="text-gray-800 mb-4">
            "Technology is nothing. What's important is that you have a faith in people, that they're basically good and smart, and if you give them tools, they'll do wonderful things with them."
        </p>
        <footer class="flex justify-between items-center">
            <div>
                <cite class="font-medium text-gray-900 not-italic">Steve Jobs</cite>
                <p class="text-sm text-gray-600">Rolling Stone Interview, 1994</p>
            </div>
            <div class="text-purple-600">
                <i class="ri-apple-fill text-2xl"></i>
            </div>
        </footer>
    </blockquote>
</div>
```

## Example 4: Pull Quote Style

```html
<div class="relative my-8">
    <div class="md:flex">
        <div class="md:w-1/3"></div>
        <blockquote class="md:w-2/3 relative z-10 p-6 md:p-8 bg-amber-50 rounded-lg shadow">
            <p class="text-xl md:text-2xl text-amber-900 font-serif leading-relaxed">
                "We don't have to be smarter than the rest. We have to be more disciplined than the rest."
            </p>
            <footer class="mt-4">
                <cite class="font-medium text-gray-900 not-italic">Warren Buffett</cite>
            </footer>
        </blockquote>
    </div>
    <div class="absolute top-0 left-0 w-24 h-24 md:w-32 md:h-32 bg-amber-200 rounded-full -z-10 -translate-x-1/3 -translate-y-1/3"></div>
</div>
```

## Example 5: Interactive Testimonial Blockquote

```html
<div class="relative overflow-hidden" id="testimonial-container">
    <div class="flex transition-transform duration-500" id="testimonial-slider">
        <!-- Testimonial 1 -->
        <blockquote class="flex-shrink-0 w-full p-6 bg-gradient-to-br from-blue-50 to-indigo-50 rounded-lg">
            <div class="flex items-center mb-4">
                <div class="flex-shrink-0">
                    <img src="https://randomuser.me/api/portraits/women/17.jpg" alt="Emma Thompson" class="w-12 h-12 rounded-full">
                </div>
                <div class="ml-4">
                    <cite class="font-medium text-gray-900 not-italic">Emma Thompson</cite>
                    <p class="text-sm text-gray-600">Designer at CreativeStudio</p>
                </div>
            </div>
            <div class="relative">
                <i class="ri-double-quotes-l absolute -top-2 -left-1 text-blue-200 text-4xl"></i>
                <p class="text-gray-700 relative z-10 pl-3">
                    Tailwind CSS has completely transformed my workflow. What used to take hours now takes minutes. The utility-first approach has made my designs more consistent and helped me focus on what matters most - creating beautiful user experiences.
                </p>
            </div>
            <div class="mt-4 flex items-center">
                <div class="flex text-yellow-400">
                    <i class="ri-star-fill"></i>
                    <i class="ri-star-fill"></i>
                    <i class="ri-star-fill"></i>
                    <i class="ri-star-fill"></i>
                    <i class="ri-star-fill"></i>
                </div>
                <span class="text-xs text-gray-500 ml-2">5.0</span>
            </div>
        </blockquote>
        
        <!-- Navigation Buttons -->
        <div class="flex justify-center mt-6 space-x-2">
            <button class="testimony-dot active w-3 h-3 rounded-full bg-blue-500" data-index="0"></button>
            <button class="testimony-dot w-3 h-3 rounded-full bg-gray-300" data-index="1"></button>
            <button class="testimony-dot w-3 h-3 rounded-full bg-gray-300" data-index="2"></button>
        </div>
    </div>
</div>
```
