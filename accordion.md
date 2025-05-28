# Accordion Component Examples

## Example 1: Simple FAQ Accordion
Use this for basic FAQ sections with clean styling and smooth animations.

```html
<div class="bg-white rounded-xl shadow-lg p-6">
    <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
        <i class="ri-question-answer-line text-blue-500 mr-3"></i>
        FAQ Accordion
    </h2>
    <div class="space-y-4">
        <div class="border border-gray-200 rounded-lg overflow-hidden">
            <button 
                onclick="toggleAccordion('faq1')" 
                class="w-full px-6 py-4 text-left font-medium text-gray-700 hover:bg-gray-50 focus:outline-none focus:bg-gray-50 flex items-center justify-between transition-colors duration-200"
            >
                <span>What is Tailwind CSS?</span>
                <i class="ri-add-line text-gray-400 text-xl transition-transform duration-200"></i>
            </button>
            <div id="faq1" class="hidden px-6 py-4 bg-gray-50 border-t border-gray-200">
                <p class="text-gray-600">Tailwind CSS is a utility-first CSS framework that provides low-level utility classes to build custom designs directly in your markup.</p>
            </div>
        </div>
    </div>
</div>
```

## Example 2: Modern FAQ with Colored Icons
Perfect for help centers and support pages with category-based color coding.

```html
<div class="bg-white rounded-xl shadow-lg p-6">
    <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
        <i class="ri-lightbulb-line text-yellow-500 mr-3"></i>
        Help Center
    </h2>
    <div class="space-y-3">
        <div class="border-l-4 border-blue-500 bg-blue-50 rounded-r-lg">
            <button 
                onclick="toggleFAQ('help1')" 
                class="w-full px-6 py-4 text-left font-medium text-blue-800 hover:bg-blue-100 focus:outline-none focus:bg-blue-100 flex items-center justify-between transition-colors duration-200"
            >
                <div class="flex items-center">
                    <i class="ri-user-line text-blue-600 mr-3"></i>
                    <span>How do I create an account?</span>
                </div>
                <i class="ri-arrow-down-s-line text-blue-600 text-xl transition-transform duration-200"></i>
            </button>
            <div id="help1" class="hidden px-6 py-4 text-blue-700">
                <p>Click the "Sign Up" button in the top right corner, fill in your details, and verify your email address.</p>
            </div>
        </div>
    </div>
</div>
```

## Example 3: Settings Panel Accordion
Ideal for configuration panels and settings pages with form elements.

```html
<div class="bg-white rounded-xl shadow-lg p-6">
    <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
        <i class="ri-settings-3-line text-gray-600 mr-3"></i>
        Settings Panel
    </h2>
    <div class="space-y-2">
        <div class="border border-gray-200 rounded-lg">
            <button 
                onclick="toggleSettings('settings1')" 
                class="w-full px-4 py-3 text-left font-medium text-gray-700 hover:bg-gray-50 focus:outline-none flex items-center transition-colors duration-200"
            >
                <i class="ri-arrow-right-s-line text-gray-400 text-lg mr-2 transition-transform duration-200"></i>
                <i class="ri-notification-3-line text-gray-500 mr-3"></i>
                <span>Notifications</span>
            </button>
            <div id="settings1" class="hidden px-4 py-3 bg-gray-50 border-t border-gray-200">
                <div class="space-y-3">
                    <label class="flex items-center">
                        <input type="checkbox" class="form-checkbox h-4 w-4 text-blue-600 rounded">
                        <span class="ml-2 text-gray-600">Email notifications</span>
                    </label>
                    <label class="flex items-center">
                        <input type="checkbox" class="form-checkbox h-4 w-4 text-blue-600 rounded" checked>
                        <span class="ml-2 text-gray-600">Push notifications</span>
                    </label>
                </div>
            </div>
        </div>
    </div>
</div>
```

## Example 4: Feature Showcase Accordion
Great for product pages and feature demonstrations with smooth height transitions.

```html
<div class="bg-gradient-to-br from-indigo-50 to-blue-50 rounded-xl shadow-lg p-6">
    <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
        <i class="ri-star-line text-indigo-500 mr-3"></i>
        Product Features
    </h2>
    <div class="space-y-3">
        <div class="bg-white rounded-lg shadow-sm overflow-hidden">
            <button 
                onclick="toggleFeature('feature1')" 
                class="w-full px-6 py-4 text-left font-medium text-gray-700 hover:bg-gray-50 focus:outline-none flex items-center justify-between transition-all duration-300"
            >
                <div class="flex items-center">
                    <div class="w-10 h-10 bg-indigo-100 rounded-lg flex items-center justify-center mr-4">
                        <i class="ri-dashboard-3-line text-indigo-600"></i>
                    </div>
                    <div>
                        <div class="font-semibold">Advanced Analytics</div>
                        <div class="text-sm text-gray-500">Track your performance in real-time</div>
                    </div>
                </div>
                <i class="ri-arrow-down-s-line text-gray-400 text-xl transition-transform duration-300"></i>
            </button>
            <div id="feature1" class="max-h-0 overflow-hidden transition-all duration-300 ease-in-out">
                <div class="px-6 py-4 bg-gray-50 border-t border-gray-100">
                    <p class="text-gray-600 mb-3">Get detailed insights into your data with our comprehensive analytics dashboard.</p>
                    <ul class="space-y-2 text-sm text-gray-600">
                        <li class="flex items-center">
                            <i class="ri-check-line text-green-500 mr-2"></i>
                            Real-time data processing
                        </li>
                    </ul>
                </div>
            </div>
        </div>
    </div>
</div>
```

## Example 5: Support Center Accordion
Perfect for customer support and help documentation with categorized styling.

```html
<div class="bg-white rounded-xl shadow-lg p-6 border-t-4 border-blue-500">
    <h2 class="text-2xl font-bold text-gray-800 mb-6 flex items-center">
        <i class="ri-customer-service-2-line text-blue-500 mr-3"></i>
        Support Center
    </h2>
    <div class="grid gap-4">
        <div class="bg-gradient-to-r from-blue-50 to-indigo-50 rounded-lg p-1">
            <div class="bg-white rounded-lg">
                <button 
                    onclick="toggleHelp('support1')" 
                    class="w-full px-6 py-4 text-left font-medium text-gray-700 hover:bg-blue-50 focus:outline-none flex items-center justify-between transition-colors duration-200 rounded-lg"
                >
                    <div class="flex items-center">
                        <div class="w-8 h-8 bg-blue-100 rounded-full flex items-center justify-center mr-4">
                            <i class="toggle-icon ri-question-line text-blue-600"></i>
                        </div>
                        <span>How to get started?</span>
                    </div>
                    <span class="bg-blue-100 text-blue-600 text-xs px-2 py-1 rounded-full">Beginner</span>
                </button>
                <div id="support1" class="hidden px-6 py-4 border-t border-blue-100">
                    <div class="bg-blue-50 rounded-lg p-4">
                        <p class="text-blue-800 mb-3">Follow these simple steps to get started with our platform:</p>
                        <ol class="list-decimal list-inside space-y-2 text-blue-700 text-sm">
                            <li>Create your account by clicking the "Sign Up" button</li>
                            <li>Verify your email address</li>
                            <li>Complete your profile setup</li>
                        </ol>
                    </div>
                </div>
            </div>
        </div>
    </div>
</div>
```
