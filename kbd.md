# KBD Component Examples

## Example 1: Basic Keyboard Keys
```html
<p class="text-gray-700 mb-3">Press <kbd class="px-2 py-1 text-xs font-semibold text-gray-800 bg-gray-200 rounded border border-gray-300 shadow-sm">Ctrl</kbd> + <kbd class="px-2 py-1 text-xs font-semibold text-gray-800 bg-gray-200 rounded border border-gray-300 shadow-sm">C</kbd> to copy text and <kbd class="px-2 py-1 text-xs font-semibold text-gray-800 bg-gray-200 rounded border border-gray-300 shadow-sm">Ctrl</kbd> + <kbd class="px-2 py-1 text-xs font-semibold text-gray-800 bg-gray-200 rounded border border-gray-300 shadow-sm">V</kbd> to paste it.</p>
<p class="text-gray-700">Press <kbd class="px-2 py-1 text-xs font-semibold text-gray-800 bg-gray-200 rounded border border-gray-300 shadow-sm">Alt</kbd> + <kbd class="px-2 py-1 text-xs font-semibold text-gray-800 bg-gray-200 rounded border border-gray-300 shadow-sm">Tab</kbd> to switch between applications.</p>
```

## Example 2: Stylized Keyboard Keys
```html
<div class="bg-gray-800 p-5 rounded-lg text-center">
  <p class="text-gray-300 mb-4">Gaming Controls</p>
  <div class="flex flex-wrap justify-center gap-2 mb-4">
    <kbd class="flex items-center justify-center w-12 h-12 text-sm font-bold text-white bg-gray-700 rounded-lg border border-gray-600 shadow-inner shadow-gray-900/50 uppercase">W</kbd>
  </div>
  <div class="flex flex-wrap justify-center gap-2">
    <kbd class="flex items-center justify-center w-12 h-12 text-sm font-bold text-white bg-gray-700 rounded-lg border border-gray-600 shadow-inner shadow-gray-900/50 uppercase">A</kbd>
    <kbd class="flex items-center justify-center w-12 h-12 text-sm font-bold text-white bg-gray-700 rounded-lg border border-gray-600 shadow-inner shadow-gray-900/50 uppercase">S</kbd>
    <kbd class="flex items-center justify-center w-12 h-12 text-sm font-bold text-white bg-gray-700 rounded-lg border border-gray-600 shadow-inner shadow-gray-900/50 uppercase">D</kbd>
  </div>
  <p class="text-gray-400 mt-4">Use WASD keys to move your character</p>
</div>
```

## Example 3: Keyboard Shortcut Guide
```html
<div class="bg-blue-50 p-5 rounded-lg">
  <h3 class="text-lg font-medium text-blue-700 mb-3">Code Editor Shortcuts</h3>
  <div class="space-y-2">
    <div class="flex items-center justify-between p-2 hover:bg-blue-100 rounded">
      <span class="text-blue-800">Save file</span>
      <div>
        <kbd class="px-2.5 py-1.5 text-xs font-semibold text-blue-800 bg-blue-200 rounded border border-blue-300 shadow-sm inline-flex items-center">
          <i class="ri-command-line mr-1"></i>
          <span>S</span>
        </kbd>
      </div>
    </div>
    <div class="flex items-center justify-between p-2 hover:bg-blue-100 rounded">
      <span class="text-blue-800">Find text</span>
      <div>
        <kbd class="px-2.5 py-1.5 text-xs font-semibold text-blue-800 bg-blue-200 rounded border border-blue-300 shadow-sm inline-flex items-center">
          <i class="ri-command-line mr-1"></i>
          <span>F</span>
        </kbd>
      </div>
    </div>
  </div>
</div>
```

## Example 4: Interactive Keyboard Keys with Animation
```html
<div class="bg-gradient-to-r from-purple-50 to-pink-50 p-5 rounded-lg text-center">
  <p class="text-gray-700 mb-4">Click on any key to see the animation</p>
  <div class="flex flex-wrap justify-center gap-3">
    <button class="transition-all active:scale-95 active:translate-y-1 focus:outline-none">
      <kbd class="flex items-center justify-center w-14 h-14 text-lg font-bold text-purple-700 bg-white rounded-xl border-2 border-purple-200 shadow-md hover:shadow-purple-300/50 hover:border-purple-300 transition-all">
        <i class="ri-arrow-left-line"></i>
      </kbd>
    </button>
    <button class="transition-all active:scale-95 active:translate-y-1 focus:outline-none">
      <kbd class="flex items-center justify-center w-14 h-14 text-lg font-bold text-purple-700 bg-white rounded-xl border-2 border-purple-200 shadow-md hover:shadow-purple-300/50 hover:border-purple-300 transition-all">
        <i class="ri-arrow-up-line"></i>
      </kbd>
    </button>
  </div>
</div>
```

## Example 5: Command Center with KBD
```html
<div class="bg-gray-900 p-5 rounded-lg">
  <div class="flex items-center justify-between border border-gray-700 rounded-md px-4 py-2 mb-4">
    <div class="flex items-center space-x-2">
      <i class="ri-search-line text-gray-500"></i>
      <span class="text-gray-400">Search commands...</span>
    </div>
    <kbd class="flex items-center gap-1 px-2 py-1 text-xs font-medium text-gray-400 bg-gray-800 rounded border border-gray-700">
      <i class="ri-command-line"></i>
      <span>K</span>
    </kbd>
  </div>
  
  <div class="space-y-1">
    <div class="flex items-center justify-between px-3 py-2 hover:bg-gray-800 rounded-md transition-colors">
      <div class="flex items-center space-x-3">
        <i class="ri-file-add-line text-blue-400"></i>
        <span class="text-gray-300">New File</span>
      </div>
      <kbd class="px-2 py-1 text-xs font-medium text-gray-400 bg-gray-800 rounded border border-gray-700">
        <i class="ri-command-line mr-1 inline-block"></i>N
      </kbd>
    </div>
  </div>
</div>
```
