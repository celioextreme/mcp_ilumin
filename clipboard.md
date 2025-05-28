# Clipboard Component Examples

## Example 1: Basic Clipboard Button
```html
<div class="relative flex items-center mt-2">
    <div class="flex-grow p-4 bg-gray-50 border border-gray-200 rounded-lg">
        <code class="text-sm text-gray-800">npm install tailwindcss</code>
    </div>
    <button 
        class="clipboard-btn ml-3 p-2 bg-blue-500 text-white rounded-md hover:bg-blue-600 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:ring-offset-2 relative"
        data-clipboard-text="npm install tailwindcss"
        onclick="copyToClipboard(this)">
        <i class="ri-clipboard-line text-lg"></i>
        <span class="clipboard-tooltip">Copy to clipboard</span>
    </button>
</div>

<script>
function copyToClipboard(button) {
    const text = button.getAttribute('data-clipboard-text');
    navigator.clipboard.writeText(text).then(() => {
        const icon = button.querySelector('i');
        
        // Change to check icon temporarily
        icon.classList.remove('ri-clipboard-line');
        icon.classList.add('ri-check-line');
        
        // Revert back after 1.5 seconds
        setTimeout(() => {
            icon.classList.remove('ri-check-line');
            icon.classList.add('ri-clipboard-line');
        }, 1500);
    });
}
</script>
```

## Example 2: Clipboard with Feedback
```html
<div class="flex items-center p-4 border border-gray-200 bg-gray-50 rounded-md">
    <div class="flex-grow">
        <div class="text-sm font-medium text-gray-500">API Key</div>
        <div class="text-gray-800 font-mono mt-1" id="api-key-text">AbC123XyZ456_789-DEF-ghI-jkL</div>
    </div>
    <div class="relative">
        <button 
            id="api-btn" 
            class="p-3 bg-gray-100 hover:bg-gray-200 text-gray-600 rounded-full focus:outline-none transition-colors duration-200 relative"
            data-clipboard-text="AbC123XyZ456_789-DEF-ghI-jkL"
            onclick="copyWithFeedback(this, 'Copied!', 'api-feedback')">
            <i id="api-icon" class="ri-clipboard-line text-lg"></i>
        </button>
        <span id="api-feedback" class="hidden absolute right-full -translate-y-1/2 top-1/2 mr-2 text-xs px-2 py-1 bg-gray-800 text-white rounded whitespace-nowrap">
            Copied!
        </span>
    </div>
</div>

<script>
function copyWithFeedback(button, message, feedbackId) {
    const text = button.getAttribute('data-clipboard-text');
    const feedback = document.getElementById(feedbackId);
    const icon = button.querySelector('i');
    
    navigator.clipboard.writeText(text).then(() => {
        // Show feedback
        feedback.classList.remove('hidden');
        feedback.classList.add('animate-fade-in');
        
        // Change icon
        icon.classList.remove('ri-clipboard-line');
        icon.classList.add('ri-check-line', 'text-green-500', 'animate-clipboard-success');
        
        // Hide feedback and revert icon after delay
        setTimeout(() => {
            feedback.classList.add('hidden');
            icon.classList.remove('ri-check-line', 'text-green-500', 'animate-clipboard-success');
            icon.classList.add('ri-clipboard-line');
        }, 2000);
    });
}
</script>
```

## Example 3: Code Block with Clipboard
```html
<div class="relative">
    <div class="absolute top-3 right-3">
        <button 
            class="px-3 py-1.5 bg-gray-700 text-white text-xs rounded-md hover:bg-gray-600 focus:outline-none focus:ring-2 focus:ring-gray-500 focus:ring-offset-2 transition-colors duration-200 flex items-center space-x-1"
            data-clipboard-target="#htmlCode"
            onclick="copyWithIcon(this)">
            <i class="ri-clipboard-line"></i>
            <span>Copy</span>
        </button>
    </div>
    <pre class="bg-gray-900 text-gray-100 p-4 rounded-lg overflow-x-auto"><code id="htmlCode" class="language-html text-sm">&lt;div class="flex flex-col"&gt;
  &lt;div class="p-4 bg-white shadow rounded-lg"&gt;
    &lt;h2 class="text-xl font-bold"&gt;Card Title&lt;/h2&gt;
    &lt;p class="mt-2 text-gray-600"&gt;
      This is a simple card with some content.
    &lt;/p&gt;
    &lt;button class="mt-4 px-4 py-2 bg-blue-500 text-white rounded-md"&gt;
      Button
    &lt;/button&gt;
  &lt;/div&gt;
&lt;/div&gt;</code></pre>
</div>

<script>
function copyWithIcon(button) {
    const targetId = button.getAttribute('data-clipboard-target');
    const text = document.querySelector(targetId).innerText;
    
    navigator.clipboard.writeText(text).then(() => {
        const icon = button.querySelector('i');
        const span = button.querySelector('span');
        
        // Change button content
        icon.classList.remove('ri-clipboard-line');
        icon.classList.add('ri-check-line');
        span.textContent = 'Copied!';
        
        // Revert after delay
        setTimeout(() => {
            icon.classList.remove('ri-check-line');
            icon.classList.add('ri-clipboard-line');
            span.textContent = 'Copy';
        }, 2000);
    });
}
</script>
```

## Example 4: Clipboard with Custom Styling
```html
<div class="bg-gradient-to-r from-blue-50 to-indigo-50 p-5 rounded-lg border border-blue-100">
    <h3 class="text-lg font-semibold text-blue-800 mb-3">Primary Style</h3>
    <div class="relative">
        <input 
            type="text" 
            value="https://tailwindcss.com/docs" 
            class="w-full py-3 pl-4 pr-14 border border-blue-300 rounded-lg focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-transparent" 
            readonly 
        />
        <button 
            class="absolute right-1 top-1 p-2 bg-blue-600 text-white rounded-md hover:bg-blue-700 transition-colors duration-200"
            data-clipboard-text="https://tailwindcss.com/docs"
            onclick="copyWithGradient(this, 'blue')">
            <i class="ri-clipboard-line text-lg"></i>
        </button>
    </div>
</div>

<script>
function copyWithGradient(button, color) {
    const text = button.getAttribute('data-clipboard-text');
    
    navigator.clipboard.writeText(text).then(() => {
        const icon = button.querySelector('i');
        const originalClass = button.className;
        
        // Change to check icon
        icon.classList.remove('ri-clipboard-line');
        icon.classList.add('ri-check-line');
        
        // Apply success style based on color
        if (color === 'blue') {
            button.className = 'absolute right-1 top-1 p-2 bg-gradient-to-r from-blue-500 to-indigo-600 text-white rounded-md transition-all duration-500';
        }
        
        // Revert back after delay
        setTimeout(() => {
            icon.classList.remove('ri-check-line');
            icon.classList.add('ri-clipboard-line');
            button.className = originalClass;
        }, 2000);
    });
}
</script>
```

## Example 5: Advanced Clipboard with Options
```html
<div class="border border-gray-200 rounded-lg overflow-hidden">
    <div class="bg-gray-50 p-4 flex items-center justify-between">
        <h3 class="font-medium text-gray-700">Configuration File</h3>
        <div class="relative" id="clipboard-dropdown-container">
            <button 
                class="px-3 py-2 bg-white border border-gray-300 rounded-md hover:bg-gray-50 focus:outline-none focus:ring-2 focus:ring-blue-500 focus:border-blue-300 flex items-center space-x-1 text-sm"
                onclick="toggleDropdown()">
                <i class="ri-clipboard-line"></i>
                <span>Copy</span>
                <i class="ri-arrow-down-s-line ml-1"></i>
            </button>
            
            <!-- Dropdown Menu -->
            <div id="clipboard-dropdown" class="hidden absolute right-0 mt-1 w-52 bg-white rounded-md shadow-lg z-10 border border-gray-200">
                <ul class="py-1">
                    <li>
                        <button 
                            class="w-full text-left px-4 py-2 hover:bg-gray-100 flex items-center text-sm text-gray-700"
                            data-clipboard-text="module.exports = { plugins: [] }"
                            onclick="copyOptionAndClose(this)">
                            <i class="ri-file-copy-line mr-2"></i>
                            Copy Basic Config
                        </button>
                    </li>
                    <!-- Additional options... -->
                </ul>
            </div>
        </div>
    </div>
    
    <!-- Code Content -->
    <div class="bg-gray-900 text-gray-100 p-4 overflow-auto max-h-64">
        <pre id="configCode">module.exports = {
  content: [
    './src/**/*.{html,js}',
  ],
  theme: {
    extend: {
      colors: {
        primary: '#3490dc',
        secondary: '#ffed4a',
        danger: '#e3342f',
      }
    }
  },
  plugins: []
}</pre>
    </div>
    
    <!-- Copy Success Message -->
    <div id="copy-success-message" class="hidden p-3 bg-green-100 border-t border-green-200 text-green-700 text-sm flex items-center">
        <i class="ri-check-line mr-2"></i>
        <span>Copied to clipboard!</span>
    </div>
</div>

<script>
function toggleDropdown() {
    const dropdown = document.getElementById('clipboard-dropdown');
    dropdown.classList.toggle('hidden');
    
    // Close when clicking outside
    document.addEventListener('click', function closeDropdown(e) {
        const container = document.getElementById('clipboard-dropdown-container');
        if (!container.contains(e.target)) {
            dropdown.classList.add('hidden');
            document.removeEventListener('click', closeDropdown);
        }
    });
}

function copyOptionAndClose(button) {
    const text = button.getAttribute('data-clipboard-text');
    const dropdown = document.getElementById('clipboard-dropdown');
    const successMessage = document.getElementById('copy-success-message');
    
    navigator.clipboard.writeText(text).then(() => {
        // Hide dropdown
        dropdown.classList.add('hidden');
        
        // Show success message
        successMessage.classList.remove('hidden');
        
        // Hide success message after delay
        setTimeout(() => {
            successMessage.classList.add('hidden');
        }, 3000);
    });
}
</script>
```
