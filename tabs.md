# Tabs Component Examples with Tailwind CSS and Remix Icons

## Example 1: Basic Tabs

```html
<div class="mb-4 border-b border-gray-200">
    <ul class="flex flex-wrap -mb-px text-sm font-medium text-center" id="basic-tabs" role="tablist">
        <li class="mr-2" role="presentation">
            <button class="inline-block p-4 border-b-2 rounded-t-lg border-blue-600 text-blue-600 active" id="profile-tab" data-tabs-target="#profile" type="button" role="tab" aria-controls="profile" aria-selected="true">Profile</button>
        </li>
        <li class="mr-2" role="presentation">
            <button class="inline-block p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300" id="dashboard-tab" data-tabs-target="#dashboard" type="button" role="tab" aria-controls="dashboard" aria-selected="false">Dashboard</button>
        </li>
        <li class="mr-2" role="presentation">
            <button class="inline-block p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300" id="settings-tab" data-tabs-target="#settings" type="button" role="tab" aria-controls="settings" aria-selected="false">Settings</button>
        </li>
        <li role="presentation">
            <button class="inline-block p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300" id="contacts-tab" data-tabs-target="#contacts" type="button" role="tab" aria-controls="contacts" aria-selected="false">Contacts</button>
        </li>
    </ul>
</div>
<div id="basic-tabs-content">
    <div class="p-4 rounded-lg bg-gray-50" id="profile" role="tabpanel" aria-labelledby="profile-tab">
        <p class="text-sm text-gray-500">This is the profile tab content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="dashboard" role="tabpanel" aria-labelledby="dashboard-tab">
        <p class="text-sm text-gray-500">This is the dashboard tab content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="settings" role="tabpanel" aria-labelledby="settings-tab">
        <p class="text-sm text-gray-500">This is the settings tab content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="contacts" role="tabpanel" aria-labelledby="contacts-tab">
        <p class="text-sm text-gray-500">This is the contacts tab content.</p>
    </div>
</div>
```

## Example 2: Tabs with Icons

```html
<div class="mb-4 border-b border-gray-200">
    <ul class="flex flex-wrap -mb-px text-sm font-medium text-center" id="icon-tabs" role="tablist">
        <li class="mr-2" role="presentation">
            <button class="inline-flex items-center p-4 border-b-2 rounded-t-lg active border-blue-600 text-blue-600" id="home-icon-tab" data-tabs-target="#home-icon" type="button" role="tab" aria-controls="home-icon" aria-selected="true">
                <i class="ri-home-4-line mr-2 text-lg"></i> Home
            </button>
        </li>
        <li class="mr-2" role="presentation">
            <button class="inline-flex items-center p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300" id="stats-icon-tab" data-tabs-target="#stats-icon" type="button" role="tab" aria-controls="stats-icon" aria-selected="false">
                <i class="ri-bar-chart-box-line mr-2 text-lg"></i> Statistics
            </button>
        </li>
        <li class="mr-2" role="presentation">
            <button class="inline-flex items-center p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300" id="users-icon-tab" data-tabs-target="#users-icon" type="button" role="tab" aria-controls="users-icon" aria-selected="false">
                <i class="ri-user-line mr-2 text-lg"></i> Users
            </button>
        </li>
        <li role="presentation">
            <button class="inline-flex items-center p-4 border-b-2 border-transparent rounded-t-lg hover:text-gray-600 hover:border-gray-300" id="settings-icon-tab" data-tabs-target="#settings-icon" type="button" role="tab" aria-controls="settings-icon" aria-selected="false">
                <i class="ri-settings-3-line mr-2 text-lg"></i> Settings
            </button>
        </li>
    </ul>
</div>
<div id="icon-tabs-content">
    <div class="p-4 rounded-lg bg-gray-50" id="home-icon" role="tabpanel" aria-labelledby="home-icon-tab">
        <h3 class="font-medium mb-2">Home Dashboard</h3>
        <p class="text-sm text-gray-500">This is the home dashboard content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="stats-icon" role="tabpanel" aria-labelledby="stats-icon-tab">
        <h3 class="font-medium mb-2">Statistics</h3>
        <p class="text-sm text-gray-500">This is the statistics content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="users-icon" role="tabpanel" aria-labelledby="users-icon-tab">
        <h3 class="font-medium mb-2">User Management</h3>
        <p class="text-sm text-gray-500">This is the user management content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="settings-icon" role="tabpanel" aria-labelledby="settings-icon-tab">
        <h3 class="font-medium mb-2">Application Settings</h3>
        <p class="text-sm text-gray-500">This is the settings content.</p>
    </div>
</div>
```

## Example 3: Pills Tabs

```html
<div class="mb-4">
    <ul class="flex flex-wrap text-sm font-medium text-center text-gray-500 border-b border-gray-200" id="pills-tabs" role="tablist">
        <li class="mr-2" role="presentation">
            <button class="inline-block px-4 py-2 text-white bg-blue-600 rounded-t-lg active" id="overview-tab" data-tabs-target="#overview" type="button" role="tab" aria-controls="overview" aria-selected="true">Overview</button>
        </li>
        <li class="mr-2" role="presentation">
            <button class="inline-block px-4 py-2 rounded-t-lg hover:text-gray-600 hover:bg-gray-50" id="features-tab" data-tabs-target="#features" type="button" role="tab" aria-controls="features" aria-selected="false">Features</button>
        </li>
        <li class="mr-2" role="presentation">
            <button class="inline-block px-4 py-2 rounded-t-lg hover:text-gray-600 hover:bg-gray-50" id="requirements-tab" data-tabs-target="#requirements" type="button" role="tab" aria-controls="requirements" aria-selected="false">Requirements</button>
        </li>
        <li role="presentation">
            <button class="inline-block px-4 py-2 rounded-t-lg hover:text-gray-600 hover:bg-gray-50" id="reviews-tab" data-tabs-target="#reviews" type="button" role="tab" aria-controls="reviews" aria-selected="false">Reviews</button>
        </li>
    </ul>
</div>
<div id="pills-tabs-content">
    <div class="p-4 rounded-lg bg-gray-50" id="overview" role="tabpanel" aria-labelledby="overview-tab">
        <h3 class="font-medium mb-2">Product Overview</h3>
        <p class="text-sm text-gray-500">This is the product overview content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="features" role="tabpanel" aria-labelledby="features-tab">
        <h3 class="font-medium mb-2">Key Features</h3>
        <p class="text-sm text-gray-500">This is the features content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="requirements" role="tabpanel" aria-labelledby="requirements-tab">
        <h3 class="font-medium mb-2">System Requirements</h3>
        <p class="text-sm text-gray-500">This is the requirements content.</p>
    </div>
    <div class="hidden p-4 rounded-lg bg-gray-50" id="reviews" role="tabpanel" aria-labelledby="reviews-tab">
        <h3 class="font-medium mb-2">Customer Reviews</h3>
        <p class="text-sm text-gray-500">This is the reviews content.</p>
    </div>
</div>
```

## Example 4: Vertical Tabs

```html
<div class="flex flex-col md:flex-row">
    <div class="w-full md:w-1/4 md:border-r border-gray-200 mb-4 md:mb-0">
        <div class="text-sm font-medium text-gray-500">
            <ul class="space-y-1" id="vertical-tabs" role="tablist">
                <li>
                    <button class="w-full py-3 px-4 text-left bg-blue-50 text-blue-600 border-l-2 border-blue-600 rounded-r-lg" id="about-tab" data-tabs-target="#about" type="button" role="tab" aria-controls="about" aria-selected="true">
                        About Us
                    </button>
                </li>
                <li>
                    <button class="w-full py-3 px-4 text-left hover:bg-gray-50 hover:text-gray-600 rounded-r-lg" id="services-tab" data-tabs-target="#services" type="button" role="tab" aria-controls="services" aria-selected="false">
                        Services
                    </button>
                </li>
                <li>
                    <button class="w-full py-3 px-4 text-left hover:bg-gray-50 hover:text-gray-600 rounded-r-lg" id="clients-tab" data-tabs-target="#clients" type="button" role="tab" aria-controls="clients" aria-selected="false">
                        Clients
                    </button>
                </li>
                <li>
                    <button class="w-full py-3 px-4 text-left hover:bg-gray-50 hover:text-gray-600 rounded-r-lg" id="contact-tab" data-tabs-target="#contact" type="button" role="tab" aria-controls="contact" aria-selected="false">
                        Contact
                    </button>
                </li>
            </ul>
        </div>
    </div>
    <div class="w-full md:w-3/4 md:pl-6">
        <div id="vertical-tabs-content">
            <div class="p-4 rounded-lg" id="about" role="tabpanel" aria-labelledby="about-tab">
                <h3 class="text-lg font-semibold mb-3">About Our Company</h3>
                <p class="text-gray-500 mb-4">This is the about content.</p>
            </div>
            <div class="hidden p-4 rounded-lg" id="services" role="tabpanel" aria-labelledby="services-tab">
                <h3 class="text-lg font-semibold mb-3">Our Services</h3>
                <p class="text-gray-500 mb-4">This is the services content.</p>
            </div>
            <div class="hidden p-4 rounded-lg" id="clients" role="tabpanel" aria-labelledby="clients-tab">
                <h3 class="text-lg font-semibold mb-3">Our Clients</h3>
                <p class="text-gray-500 mb-4">This is the clients content.</p>
            </div>
            <div class="hidden p-4 rounded-lg" id="contact" role="tabpanel" aria-labelledby="contact-tab">
                <h3 class="text-lg font-semibold mb-3">Get in Touch</h3>
                <p class="text-gray-500 mb-4">This is the contact content.</p>
            </div>
        </div>
    </div>
</div>
```

## Example 5: Custom Styled Tabs

```html
<div class="mb-6">
    <div class="flex justify-center">
        <div class="inline-flex p-1 bg-gray-100 rounded-xl" id="custom-tabs" role="tablist">
            <button class="px-5 py-2 rounded-lg bg-purple-600 text-white shadow" id="design-tab" data-tabs-target="#design" type="button" role="tab" aria-controls="design" aria-selected="true">Design</button>
            <button class="px-5 py-2 text-gray-700 hover:text-gray-900" id="code-tab" data-tabs-target="#code" type="button" role="tab" aria-controls="code" aria-selected="false">Code</button>
            <button class="px-5 py-2 text-gray-700 hover:text-gray-900" id="preview-tab" data-tabs-target="#preview" type="button" role="tab" aria-controls="preview" aria-selected="false">Preview</button>
        </div>
    </div>
</div>

<div id="custom-tabs-content">
    <div class="p-6 bg-gray-50 rounded-lg" id="design" role="tabpanel" aria-labelledby="design-tab">
        <div class="flex items-center justify-between mb-4">
            <h3 class="text-lg font-semibold">Design Canvas</h3>
            <div class="flex space-x-2">
                <button class="p-2 bg-white rounded-lg shadow hover:bg-gray-50">
                    <i class="ri-zoom-in-line"></i>
                </button>
                <button class="p-2 bg-white rounded-lg shadow hover:bg-gray-50">
                    <i class="ri-zoom-out-line"></i>
                </button>
                <button class="p-2 bg-white rounded-lg shadow hover:bg-gray-50">
                    <i class="ri-refresh-line"></i>
                </button>
            </div>
        </div>
        <div class="bg-white border border-gray-200 rounded-lg h-64 flex items-center justify-center">
            <p class="text-gray-500">Design workspace would appear here</p>
        </div>
    </div>
    <div class="hidden p-6 bg-gray-50 rounded-lg" id="code" role="tabpanel" aria-labelledby="code-tab">
        <!-- Code tab content -->
    </div>
    <div class="hidden p-6 bg-gray-50 rounded-lg" id="preview" role="tabpanel" aria-labelledby="preview-tab">
        <!-- Preview tab content -->
    </div>
</div>

<script>
    // Simple tabs functionality
    function setupTabs(tabsGroup) {
        let tabElements = document.querySelectorAll(`#${tabsGroup} button`);
        tabElements.forEach(tabEl => {
            tabEl.addEventListener('click', function() {
                // Hide all content sections
                document.querySelectorAll(`#${tabsGroup}-content > div`).forEach(content => {
                    content.classList.add('hidden');
                });
                
                // Remove active class from all tabs
                document.querySelectorAll(`#${tabsGroup} button`).forEach(tab => {
                    // ... tab class removal logic
                });
                
                // Show the clicked tab content
                const target = this.getAttribute('data-tabs-target').replace('#', '');
                document.getElementById(target).classList.remove('hidden');
                
                // Add active class to clicked tab
                this.setAttribute('aria-selected', 'true');
                // ... tab class addition logic
            });
        });
    }
    
    // Initialize all tab groups
    setupTabs('basic-tabs');
    setupTabs('icon-tabs');
    setupTabs('pills-tabs');
    setupTabs('vertical-tabs');
    setupTabs('custom-tabs');
</script>
```
