# Table Component Examples with Tailwind CSS and Remix Icons

## Example 1: Simple Data Table

```html
<div class="overflow-x-auto">
    <table class="w-full text-sm text-left text-gray-500">
        <thead class="text-xs text-gray-700 uppercase bg-gray-50">
            <tr>
                <th scope="col" class="px-6 py-3">
                    Product name
                </th>
                <th scope="col" class="px-6 py-3">
                    Category
                </th>
                <th scope="col" class="px-6 py-3">
                    Price
                </th>
                <th scope="col" class="px-6 py-3">
                    Stock
                </th>
                <th scope="col" class="px-6 py-3">
                    Action
                </th>
            </tr>
        </thead>
        <tbody>
            <tr class="bg-white border-b hover:bg-gray-50">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                    Apple MacBook Pro 17"
                </th>
                <td class="px-6 py-4">
                    Laptop
                </td>
                <td class="px-6 py-4">
                    $2999
                </td>
                <td class="px-6 py-4">
                    18
                </td>
                <td class="px-6 py-4">
                    <a href="#" class="font-medium text-blue-600 hover:underline">Edit</a>
                </td>
            </tr>
            <tr class="bg-white border-b hover:bg-gray-50">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                    Microsoft Surface Pro
                </th>
                <td class="px-6 py-4">
                    Laptop PC
                </td>
                <td class="px-6 py-4">
                    $1999
                </td>
                <td class="px-6 py-4">
                    10
                </td>
                <td class="px-6 py-4">
                    <a href="#" class="font-medium text-blue-600 hover:underline">Edit</a>
                </td>
            </tr>
            <tr class="bg-white hover:bg-gray-50">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                    Magic Mouse 2
                </th>
                <td class="px-6 py-4">
                    Accessories
                </td>
                <td class="px-6 py-4">
                    $99
                </td>
                <td class="px-6 py-4">
                    23
                </td>
                <td class="px-6 py-4">
                    <a href="#" class="font-medium text-blue-600 hover:underline">Edit</a>
                </td>
            </tr>
        </tbody>
    </table>
</div>
```

## Example 2: Striped Table with Status

```html
<div class="overflow-x-auto">
    <table class="w-full text-sm text-left text-gray-500">
        <thead class="text-xs text-white uppercase bg-blue-600">
            <tr>
                <th scope="col" class="px-6 py-3">
                    Order ID
                </th>
                <th scope="col" class="px-6 py-3">
                    Customer
                </th>
                <th scope="col" class="px-6 py-3">
                    Date
                </th>
                <th scope="col" class="px-6 py-3">
                    Total
                </th>
                <th scope="col" class="px-6 py-3">
                    Status
                </th>
            </tr>
        </thead>
        <tbody>
            <tr class="bg-white border-b hover:bg-blue-50">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                    #ORD-001234
                </th>
                <td class="px-6 py-4">
                    Sarah Johnson
                </td>
                <td class="px-6 py-4">
                    May 15, 2023
                </td>
                <td class="px-6 py-4 font-medium">
                    $349.99
                </td>
                <td class="px-6 py-4">
                    <span class="px-2 py-1 text-xs font-semibold rounded-full bg-green-100 text-green-800">
                        Completed
                    </span>
                </td>
            </tr>
            <tr class="bg-gray-50 border-b hover:bg-blue-50">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                    #ORD-001235
                </th>
                <td class="px-6 py-4">
                    John Smith
                </td>
                <td class="px-6 py-4">
                    May 16, 2023
                </td>
                <td class="px-6 py-4 font-medium">
                    $129.50
                </td>
                <td class="px-6 py-4">
                    <span class="px-2 py-1 text-xs font-semibold rounded-full bg-yellow-100 text-yellow-800">
                        Processing
                    </span>
                </td>
            </tr>
            <tr class="bg-white border-b hover:bg-blue-50">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                    #ORD-001236
                </th>
                <td class="px-6 py-4">
                    Emily Davis
                </td>
                <td class="px-6 py-4">
                    May 16, 2023
                </td>
                <td class="px-6 py-4 font-medium">
                    $75.25
                </td>
                <td class="px-6 py-4">
                    <span class="px-2 py-1 text-xs font-semibold rounded-full bg-green-100 text-green-800">
                        Completed
                    </span>
                </td>
            </tr>
        </tbody>
    </table>
</div>
```

## Example 3: Table with Search, Filter, and Pagination

```html
<!-- Table Controls -->
<div class="flex flex-col md:flex-row justify-between items-center mb-4 space-y-3 md:space-y-0">
    <!-- Search -->
    <div class="relative w-full md:w-1/3">
        <div class="absolute inset-y-0 left-0 flex items-center pl-3 pointer-events-none">
            <i class="ri-search-line text-gray-500"></i>
        </div>
        <input type="text" class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full pl-10 p-2.5" placeholder="Search users">
    </div>
    
    <!-- Filters -->
    <div class="flex items-center space-x-3">
        <div>
            <select class="bg-gray-50 border border-gray-300 text-gray-900 text-sm rounded-lg focus:ring-blue-500 focus:border-blue-500 block w-full p-2.5">
                <option selected>All Roles</option>
                <option value="admin">Admin</option>
                <option value="editor">Editor</option>
                <option value="viewer">Viewer</option>
            </select>
        </div>
        <button class="inline-flex items-center text-gray-500 bg-white border border-gray-300 focus:outline-none hover:bg-gray-100 focus:ring-4 focus:ring-gray-200 font-medium rounded-lg text-sm px-3 py-2.5">
            <i class="ri-filter-3-line mr-2"></i> Filter
        </button>
        <button class="inline-flex items-center text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:ring-blue-300 font-medium rounded-lg text-sm px-3 py-2.5">
            <i class="ri-add-line mr-2"></i> Add User
        </button>
    </div>
</div>

<!-- Table -->
<div class="overflow-x-auto">
    <table class="w-full text-sm text-left text-gray-500">
        <thead class="text-xs text-gray-700 uppercase bg-gray-50">
            <tr>
                <th scope="col" class="p-4">
                    <div class="flex items-center">
                        <input id="checkbox-all" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500">
                    </div>
                </th>
                <th scope="col" class="px-6 py-3">Name</th>
                <th scope="col" class="px-6 py-3">Email</th>
                <th scope="col" class="px-6 py-3">Role</th>
                <th scope="col" class="px-6 py-3">Status</th>
                <th scope="col" class="px-6 py-3">Action</th>
            </tr>
        </thead>
        <tbody>
            <tr class="bg-white border-b hover:bg-gray-50">
                <td class="w-4 p-4">
                    <div class="flex items-center">
                        <input id="checkbox-1" type="checkbox" class="w-4 h-4 text-blue-600 bg-gray-100 border-gray-300 rounded focus:ring-blue-500">
                    </div>
                </td>
                <th scope="row" class="flex items-center px-6 py-4 text-gray-900 whitespace-nowrap">
                    <img class="w-10 h-10 rounded-full" src="https://randomuser.me/api/portraits/men/1.jpg" alt="User Avatar">
                    <div class="pl-3">
                        <div class="text-base font-semibold">Neil Sims</div>
                        <div class="font-normal text-gray-500">United States</div>
                    </div>
                </th>
                <td class="px-6 py-4">neil.sims@example.com</td>
                <td class="px-6 py-4">
                    <span class="px-2 py-1 text-xs font-semibold rounded bg-indigo-100 text-indigo-800">Admin</span>
                </td>
                <td class="px-6 py-4">
                    <div class="flex items-center">
                        <div class="h-2.5 w-2.5 rounded-full bg-green-500 mr-2"></div> Online
                    </div>
                </td>
                <td class="px-6 py-4">
                    <div class="flex space-x-2">
                        <a href="#" class="font-medium text-blue-600 hover:underline">Edit</a>
                        <a href="#" class="font-medium text-red-600 hover:underline">Delete</a>
                    </div>
                </td>
            </tr>
        </tbody>
    </table>
</div>

<!-- Pagination -->
<div class="flex flex-col md:flex-row justify-between items-center mt-4 space-y-3 md:space-y-0">
    <span class="text-sm text-gray-700">
        Showing <span class="font-semibold text-gray-900">1</span> to <span class="font-semibold text-gray-900">3</span> of <span class="font-semibold text-gray-900">10</span> entries
    </span>
    <div class="inline-flex mt-2 md:mt-0">
        <button class="flex items-center justify-center px-4 h-10 text-base font-medium text-gray-500 bg-white border border-gray-300 rounded-l-lg hover:bg-gray-100 hover:text-gray-700">
            <i class="ri-arrow-left-s-line"></i>
            Previous
        </button>
        <button class="flex items-center justify-center px-4 h-10 ml-3 text-base font-medium text-gray-500 bg-white border border-gray-300 rounded-r-lg hover:bg-gray-100 hover:text-gray-700">
            Next
            <i class="ri-arrow-right-s-line"></i>
        </button>
    </div>
</div>
```

## Example 4: Expandable Table Rows

```html
<div class="overflow-x-auto">
    <table class="w-full text-sm text-left text-gray-500">
        <thead class="text-xs text-gray-700 uppercase bg-gray-50">
            <tr>
                <th scope="col" class="px-6 py-3">
                    Project
                </th>
                <th scope="col" class="px-6 py-3">
                    Status
                </th>
                <th scope="col" class="px-6 py-3">
                    Progress
                </th>
                <th scope="col" class="px-6 py-3">
                    Due Date
                </th>
                <th scope="col" class="px-6 py-3">
                    Team
                </th>
                <th scope="col" class="px-6 py-3">
                    <span class="sr-only">Expand</span>
                </th>
            </tr>
        </thead>
        <tbody>
            <!-- Row 1 -->
            <tr class="bg-white border-b hover:bg-gray-50">
                <th scope="row" class="px-6 py-4 font-medium text-gray-900 whitespace-nowrap">
                    Website Redesign
                </th>
                <td class="px-6 py-4">
                    <span class="px-2 py-1 text-xs font-semibold rounded-full bg-yellow-100 text-yellow-800">In Progress</span>
                </td>
                <td class="px-6 py-4">
                    <div class="w-full bg-gray-200 rounded-full h-2.5">
                        <div class="bg-blue-600 h-2.5 rounded-full" style="width: 65%"></div>
                    </div>
                    <span class="text-xs mt-1 inline-block">65%</span>
                </td>
                <td class="px-6 py-4">
                    June 15, 2023
                </td>
                <td class="px-6 py-4">
                    <div class="flex -space-x-2">
                        <img class="w-7 h-7 rounded-full border-2 border-white" src="https://randomuser.me/api/portraits/men/4.jpg" alt="">
                        <img class="w-7 h-7 rounded-full border-2 border-white" src="https://randomuser.me/api/portraits/women/5.jpg" alt="">
                        <img class="w-7 h-7 rounded-full border-2 border-white" src="https://randomuser.me/api/portraits/men/6.jpg" alt="">
                    </div>
                </td>
                <td class="px-6 py-4 text-right">
                    <button onclick="toggleRow('details-1')" class="font-medium text-blue-600 hover:underline flex items-center justify-end w-full">
                        <i class="ri-arrow-down-s-line text-lg"></i>
                    </button>
                </td>
            </tr>
            <!-- Expandable Content for Row 1 -->
            <tr class="hidden bg-gray-50" id="details-1">
                <td colspan="6" class="px-6 py-4">
                    <div class="grid grid-cols-1 md:grid-cols-3 gap-4">
                        <div>
                            <h5 class="font-semibold mb-2">Project Description</h5>
                            <p class="text-gray-600 text-sm">Complete overhaul of company website including new home page, product pages, and checkout flow.</p>
                        </div>
                        <div>
                            <h5 class="font-semibold mb-2">Milestones</h5>
                            <ul class="list-disc pl-5 text-sm text-gray-600">
                                <li>Homepage Design <span class="text-green-600">✓</span></li>
                                <li>Product Page Templates <span class="text-green-600">✓</span></li>
                                <li>Checkout Page - in progress</li>
                                <li>Mobile Responsive Design - pending</li>
                            </ul>
                        </div>
                        <div>
                            <h5 class="font-semibold mb-2">Latest Comments</h5>
                            <div class="text-sm">
                                <div class="mb-2">
                                    <span class="font-medium text-gray-900">Sarah J.</span>:
                                    <span class="text-gray-600">Updated the product page mockups</span>
                                </div>
                                <div>
                                    <span class="font-medium text-gray-900">Mike T.</span>:
                                    <span class="text-gray-600">Need feedback on the checkout form</span>
                                </div>
                            </div>
                        </div>
                    </div>
                </td>
            </tr>
        </tbody>
    </table>
</div>

<script>
    function toggleRow(rowId) {
        const row = document.getElementById(rowId);
        const button = event.currentTarget;
        const icon = button.querySelector('i');
        
        if (row.classList.contains('hidden')) {
            row.classList.remove('hidden');
            icon.classList.remove('ri-arrow-down-s-line');
            icon.classList.add('ri-arrow-up-s-line');
        } else {
            row.classList.add('hidden');
            icon.classList.remove('ri-arrow-up-s-line');
            icon.classList.add('ri-arrow-down-s-line');
        }
    }
</script>
```

## Example 5: Responsive Card Table for Mobile

```html
<div class="grid grid-cols-1 gap-4">
    <!-- Table Header - Only visible on desktop -->
    <div class="hidden md:grid grid-cols-5 gap-4 text-xs font-medium text-gray-700 uppercase bg-gray-50 p-4 rounded-lg">
        <div>Employee</div>
        <div>Position</div>
        <div>Department</div>
        <div>Location</div>
        <div class="text-right">Salary</div>
    </div>
    
    <!-- Table Row 1 - Card on mobile, row on desktop -->
    <div class="bg-white border rounded-lg shadow-sm p-4 md:p-0 md:shadow-none md:border-0 md:rounded-none md:grid md:grid-cols-5 md:gap-4 md:items-center hover:bg-gray-50">
        <div class="flex items-center mb-3 md:mb-0">
            <img class="w-10 h-10 rounded-full mr-3" src="https://randomuser.me/api/portraits/men/11.jpg" alt="User Avatar">
            <div>
                <p class="font-medium text-gray-900">Thomas Wilson</p>
                <p class="text-sm text-gray-500 md:hidden">thomas.wilson@example.com</p>
            </div>
        </div>
        <div class="mb-2 md:mb-0">
            <span class="md:hidden font-medium text-gray-900">Position: </span>
            <span>Senior Developer</span>
        </div>
        <div class="mb-2 md:mb-0">
            <span class="md:hidden font-medium text-gray-900">Department: </span>
            <span>Engineering</span>
        </div>
        <div class="mb-2 md:mb-0">
            <span class="md:hidden font-medium text-gray-900">Location: </span>
            <span>San Francisco, CA</span>
        </div>
        <div class="md:text-right font-medium text-gray-900">
            <span class="md:hidden font-medium text-gray-900">Salary: </span>
            <span>$125,000</span>
        </div>
    </div>
    
    <!-- Table Row 2 - Card on mobile, row on desktop -->
    <div class="bg-white border rounded-lg shadow-sm p-4 md:p-0 md:shadow-none md:border-0 md:rounded-none md:grid md:grid-cols-5 md:gap-4 md:items-center hover:bg-gray-50">
        <div class="flex items-center mb-3 md:mb-0">
            <img class="w-10 h-10 rounded-full mr-3" src="https://randomuser.me/api/portraits/women/12.jpg" alt="User Avatar">
            <div>
                <p class="font-medium text-gray-900">Amanda Johnson</p>
                <p class="text-sm text-gray-500 md:hidden">amanda.johnson@example.com</p>
            </div>
        </div>
        <div class="mb-2 md:mb-0">
            <span class="md:hidden font-medium text-gray-900">Position: </span>
            <span>Product Manager</span>
        </div>
        <div class="mb-2 md:mb-0">
            <span class="md:hidden font-medium text-gray-900">Department: </span>
            <span>Product</span>
        </div>
        <div class="mb-2 md:mb-0">
            <span class="md:hidden font-medium text-gray-900">Location: </span>
            <span>New York, NY</span>
        </div>
        <div class="md:text-right font-medium text-gray-900">
            <span class="md:hidden font-medium text-gray-900">Salary: </span>
            <span>$110,000</span>
        </div>
    </div>
</div>
```
