# Rating Component Examples

## Example 1: Basic Star Rating
```html
<div class="flex flex-col space-y-4">
    <div class="space-y-2">
        <p class="text-gray-700">Default rating display:</p>
        <div class="flex items-center">
            <div class="flex items-center star-rating">
                <i class="ri-star-fill text-yellow-400 text-2xl"></i>
                <i class="ri-star-fill text-yellow-400 text-2xl"></i>
                <i class="ri-star-fill text-yellow-400 text-2xl"></i>
                <i class="ri-star-fill text-gray-300 text-2xl"></i>
                <i class="ri-star-fill text-gray-300 text-2xl"></i>
            </div>
            <span class="ml-2 text-gray-600 font-medium">3.0</span>
        </div>
    </div>
    
    <div class="space-y-2">
        <p class="text-gray-700">Interactive rating:</p>
        <div class="flex items-center">
            <div class="flex items-center star-rating rating-hover">
                <span class="star"><i class="ri-star-fill text-gray-300 text-2xl"></i></span>
                <span class="star"><i class="ri-star-fill text-gray-300 text-2xl"></i></span>
                <span class="star"><i class="ri-star-fill text-gray-300 text-2xl"></i></span>
                <span class="star"><i class="ri-star-fill text-gray-300 text-2xl"></i></span>
                <span class="star"><i class="ri-star-fill text-gray-300 text-2xl"></i></span>
            </div>
            <span class="ml-2 text-gray-600 font-medium rating-value">0.0</span>
        </div>
    </div>
</div>
```

## Example 2: Emoji Rating
```html
<div class="space-y-6">
    <p class="text-gray-700">How was your experience?</p>
    
    <div class="flex justify-center space-x-6 emoji-rating">
        <button class="flex flex-col items-center space-y-2 transition-all duration-200 transform hover:scale-110 focus:outline-none group">
            <div class="p-3 bg-red-100 rounded-full text-3xl">
                <i class="ri-emotion-unhappy-line text-red-500 group-hover:text-red-600"></i>
            </div>
            <span class="text-sm font-medium text-gray-700 group-hover:text-red-600">Poor</span>
        </button>
        
        <button class="flex flex-col items-center space-y-2 transition-all duration-200 transform hover:scale-110 focus:outline-none group">
            <div class="p-3 bg-orange-100 rounded-full text-3xl">
                <i class="ri-emotion-normal-line text-orange-500 group-hover:text-orange-600"></i>
            </div>
            <span class="text-sm font-medium text-gray-700 group-hover:text-orange-600">Okay</span>
        </button>
        
        <button class="flex flex-col items-center space-y-2 transition-all duration-200 transform hover:scale-110 focus:outline-none group">
            <div class="p-3 bg-yellow-100 rounded-full text-3xl">
                <i class="ri-emotion-line text-yellow-500 group-hover:text-yellow-600"></i>
            </div>
            <span class="text-sm font-medium text-gray-700 group-hover:text-yellow-600">Good</span>
        </button>
        
        <button class="flex flex-col items-center space-y-2 transition-all duration-200 transform hover:scale-110 focus:outline-none group">
            <div class="p-3 bg-green-100 rounded-full text-3xl">
                <i class="ri-emotion-happy-line text-green-500 group-hover:text-green-600"></i>
            </div>
            <span class="text-sm font-medium text-gray-700 group-hover:text-green-600">Great</span>
        </button>
        
        <button class="flex flex-col items-center space-y-2 transition-all duration-200 transform hover:scale-110 focus:outline-none group">
            <div class="p-3 bg-primary-100 rounded-full text-3xl">
                <i class="ri-emotion-laugh-line text-primary-500 group-hover:text-primary-600"></i>
            </div>
            <span class="text-sm font-medium text-gray-700 group-hover:text-primary-600">Amazing</span>
        </button>
    </div>
</div>
```

## Example 3: Interactive Animated Rating
```html
<div class="space-y-4">
    <p class="text-gray-700">Rate this product:</p>
    
    <div class="flex items-center">
        <div class="flex items-center star-rating animate-rating" id="animated-rating">
            <span class="star" data-value="1"><i class="ri-star-fill text-gray-300 text-3xl"></i></span>
            <span class="star" data-value="2"><i class="ri-star-fill text-gray-300 text-3xl"></i></span>
            <span class="star" data-value="3"><i class="ri-star-fill text-gray-300 text-3xl"></i></span>
            <span class="star" data-value="4"><i class="ri-star-fill text-gray-300 text-3xl"></i></span>
            <span class="star" data-value="5"><i class="ri-star-fill text-gray-300 text-3xl"></i></span>
        </div>
        <span class="ml-3 text-lg font-semibold text-gray-700" id="rating-description">Select a rating</span>
    </div>

    <div class="mt-4 flex items-center">
        <span class="text-sm font-medium text-gray-600">Your rating: </span>
        <span class="ml-2 text-sm font-bold text-gray-800" id="rating-value">Not rated yet</span>
    </div>
</div>
```

## Example 4: Rating Cards with Stats
```html
<div class="grid grid-cols-1 md:grid-cols-2 gap-6">
    <!-- Product Rating Card -->
    <div class="border rounded-lg p-4 bg-gray-50">
        <div class="flex items-start gap-4">
            <div class="w-24 h-24 bg-white rounded-md flex items-center justify-center shadow">
                <i class="ri-headphone-line text-4xl text-gray-700"></i>
            </div>
            <div class="flex-1">
                <h3 class="font-semibold text-lg">Premium Headphones</h3>
                <div class="flex items-center mt-1">
                    <div class="flex">
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-half-fill text-yellow-400"></i>
                    </div>
                    <span class="ml-2 text-sm font-medium">4.5</span>
                    <span class="ml-1 text-sm text-gray-500">(2,548 reviews)</span>
                </div>
                <div class="mt-3">
                    <div class="flex items-center text-sm">
                        <span class="w-16">5 stars</span>
                        <div class="flex-1 h-2 mx-2 bg-gray-200 rounded-full">
                            <div class="h-2 bg-yellow-400 rounded-full" style="width: 75%"></div>
                        </div>
                        <span class="w-8 text-right">75%</span>
                    </div>
                    <!-- Other star ratings... -->
                </div>
            </div>
        </div>
    </div>

    <!-- App Rating Card -->
    <div class="border rounded-lg p-4 bg-gradient-to-br from-blue-50 to-indigo-50">
        <div class="text-center">
            <div class="inline-block p-3 bg-white rounded-full shadow mb-3">
                <i class="ri-app-store-line text-3xl text-indigo-600"></i>
            </div>
            <h3 class="font-semibold text-lg">Mobile App Rating</h3>
            
            <div class="flex items-center justify-center mt-2">
                <span class="text-4xl font-bold text-indigo-600">4.8</span>
                <div class="flex flex-col items-start ml-2">
                    <div class="flex">
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-fill text-yellow-400"></i>
                        <i class="ri-star-fill text-yellow-400"></i>
                    </div>
                    <span class="text-xs text-gray-500">12,385 ratings</span>
                </div>
            </div>
            
            <div class="mt-4 grid grid-cols-5 gap-1">
                <!-- Star distribution bars... -->
            </div>
        </div>
    </div>
</div>
```

## Example 5: Custom Rating with Categories
```html
<form class="space-y-6">
    <div class="space-y-4">
        <div class="border-b pb-3">
            <div class="flex items-center justify-between">
                <h3 class="font-medium">Food Quality</h3>
                <div class="flex category-rating" id="food-rating">
                    <button type="button" class="text-gray-300 hover:text-yellow-400 transition-colors p-1" data-value="1">
                        <i class="ri-knife-line text-xl"></i>
                    </button>
                    <button type="button" class="text-gray-300 hover:text-yellow-400 transition-colors p-1" data-value="2">
                        <i class="ri-knife-line text-xl"></i>
                    </button>
                    <button type="button" class="text-gray-300 hover:text-yellow-400 transition-colors p-1" data-value="3">
                        <i class="ri-knife-line text-xl"></i>
                    </button>
                    <button type="button" class="text-gray-300 hover:text-yellow-400 transition-colors p-1" data-value="4">
                        <i class="ri-knife-line text-xl"></i>
                    </button>
                    <button type="button" class="text-gray-300 hover:text-yellow-400 transition-colors p-1" data-value="5">
                        <i class="ri-knife-line text-xl"></i>
                    </button>
                </div>
            </div>
        </div>
        
        <!-- Other categories... -->
        
        <div class="mt-4">
            <label for="review" class="block text-sm font-medium text-gray-700 mb-1">Your Comments</label>
            <textarea id="review" rows="3" class="w-full px-3 py-2 border border-gray-300 rounded-md shadow-sm focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-blue-500"></textarea>
        </div>
        
        <div class="pt-2">
            <button type="button" class="w-full bg-blue-600 text-white py-2 px-4 rounded-md hover:bg-blue-700 transition-colors focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2">
                Submit Review
            </button>
        </div>
    </div>
</form>
```
