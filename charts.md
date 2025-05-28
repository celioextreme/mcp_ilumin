# Chart Examples with Tailwind CSS and Chart.js

## Example 1: Line Chart
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <div class="flex justify-between items-center mb-4">
        <h2 class="text-xl font-semibold flex items-center text-blue-600">
            <i class="ri-line-chart-line text-xl mr-2"></i> Example 1: Line Chart
        </h2>
        <div class="inline-flex rounded-md shadow-sm" role="group">
            <button type="button" class="px-4 py-2 text-sm font-medium text-blue-700 bg-white border border-gray-200 rounded-l-lg hover:bg-gray-100 focus:z-10">Weekly</button>
            <button type="button" class="px-4 py-2 text-sm font-medium text-white bg-blue-600 border border-blue-600 hover:bg-blue-700 focus:z-10">Monthly</button>
            <button type="button" class="px-4 py-2 text-sm font-medium text-blue-700 bg-white border border-gray-200 rounded-r-lg hover:bg-gray-100 focus:z-10">Yearly</button>
        </div>
    </div>
    <p class="text-gray-600 mb-6">Website traffic overview for the last 6 months</p>
    <div>
        <canvas id="lineChart" class="w-full"></canvas>
    </div>
</div>

<script>
// Line Chart
const lineCtx = document.getElementById('lineChart').getContext('2d');
const lineChart = new Chart(lineCtx, {
    type: 'line',
    data: {
        labels: ['January', 'February', 'March', 'April', 'May', 'June'],
        datasets: [
            {
                label: 'Unique Visitors',
                data: [5000, 6000, 5500, 7500, 8000, 9000],
                borderColor: '#3b82f6',
                backgroundColor: 'rgba(59, 130, 246, 0.1)',
                tension: 0.3,
                fill: true
            },
            {
                label: 'Page Views',
                data: [12000, 15000, 13500, 16000, 18000, 22000],
                borderColor: '#10b981',
                backgroundColor: 'rgba(16, 185, 129, 0.05)',
                tension: 0.3,
                fill: true
            }
        ]
    },
    options: {
        responsive: true,
        maintainAspectRatio: false,
        plugins: {
            legend: {
                position: 'top',
                labels: {
                    usePointStyle: true,
                    boxWidth: 8
                }
            }
        },
        scales: {
            y: {
                beginAtZero: true,
                grid: {
                    color: 'rgba(229, 231, 235, 0.5)'
                }
            },
            x: {
                grid: {
                    display: false
                }
            }
        }
    }
});
</script>
```

## Example 2: Bar Chart
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-bar-chart-horizontal-line text-xl mr-2"></i> Example 2: Bar Chart
    </h2>
    <p class="text-gray-600 mb-6">Monthly revenue breakdown by product category</p>
    <div>
        <canvas id="barChart" class="w-full"></canvas>
    </div>
</div>

<script>
// Bar Chart
const barCtx = document.getElementById('barChart').getContext('2d');
const barChart = new Chart(barCtx, {
    type: 'bar',
    data: {
        labels: ['Electronics', 'Clothing', 'Home', 'Beauty', 'Books', 'Sports'],
        datasets: [
            {
                label: 'Revenue (USD)',
                data: [12500, 8300, 5400, 7200, 3800, 4600],
                backgroundColor: [
                    'rgba(59, 130, 246, 0.8)',
                    'rgba(217, 70, 239, 0.8)',
                    'rgba(16, 185, 129, 0.8)',
                    'rgba(245, 158, 11, 0.8)',
                    'rgba(239, 68, 68, 0.8)',
                    'rgba(76, 29, 149, 0.8)'
                ],
                borderColor: [
                    'rgba(59, 130, 246, 1)',
                    'rgba(217, 70, 239, 1)',
                    'rgba(16, 185, 129, 1)',
                    'rgba(245, 158, 11, 1)',
                    'rgba(239, 68, 68, 1)',
                    'rgba(76, 29, 149, 1)'
                ],
                borderWidth: 1
            }
        ]
    },
    options: {
        responsive: true,
        maintainAspectRatio: false,
        plugins: {
            legend: {
                display: false
            }
        },
        scales: {
            y: {
                beginAtZero: true,
                grid: {
                    color: 'rgba(229, 231, 235, 0.5)'
                },
                ticks: {
                    callback: function(value) {
                        return '$' + value.toLocaleString();
                    }
                }
            },
            x: {
                grid: {
                    display: false
                }
            }
        }
    }
});
</script>
```

## Example 3: Pie & Doughnut Charts
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-pie-chart-line text-xl mr-2"></i> Example 3: Pie & Doughnut Charts
    </h2>
    <div class="grid grid-cols-1 md:grid-cols-2 gap-8">
        <!-- Pie Chart -->
        <div>
            <h3 class="text-lg font-medium mb-4 text-gray-900">Customer Demographics</h3>
            <div class="h-64">
                <canvas id="pieChart"></canvas>
            </div>
        </div>
        
        <!-- Doughnut Chart -->
        <div>
            <h3 class="text-lg font-medium mb-4 text-gray-900">Traffic Sources</h3>
            <div class="h-64">
                <canvas id="doughnutChart"></canvas>
            </div>
        </div>
    </div>
</div>

<script>
// Pie Chart
const pieCtx = document.getElementById('pieChart').getContext('2d');
const pieChart = new Chart(pieCtx, {
    type: 'pie',
    data: {
        labels: ['18-24', '25-34', '35-44', '45-54', '55+'],
        datasets: [{
            data: [15, 30, 25, 18, 12],
            backgroundColor: [
                'rgba(59, 130, 246, 0.8)',
                'rgba(16, 185, 129, 0.8)',
                'rgba(245, 158, 11, 0.8)',
                'rgba(217, 70, 239, 0.8)',
                'rgba(239, 68, 68, 0.8)'
            ],
            borderColor: [
                'rgba(59, 130, 246, 1)',
                'rgba(16, 185, 129, 1)',
                'rgba(245, 158, 11, 1)',
                'rgba(217, 70, 239, 1)',
                'rgba(239, 68, 68, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        responsive: true,
        maintainAspectRatio: false,
        plugins: {
            legend: {
                position: 'bottom',
                labels: {
                    usePointStyle: true,
                    boxWidth: 8,
                    font: {
                        size: 11
                    }
                }
            }
        }
    }
});

// Doughnut Chart
const doughnutCtx = document.getElementById('doughnutChart').getContext('2d');
const doughnutChart = new Chart(doughnutCtx, {
    type: 'doughnut',
    data: {
        labels: ['Organic Search', 'Direct', 'Social Media', 'Referral', 'Email'],
        datasets: [{
            data: [40, 25, 15, 10, 10],
            backgroundColor: [
                'rgba(16, 185, 129, 0.8)',
                'rgba(59, 130, 246, 0.8)',
                'rgba(245, 158, 11, 0.8)',
                'rgba(217, 70, 239, 0.8)',
                'rgba(239, 68, 68, 0.8)'
            ],
            borderColor: [
                'rgba(16, 185, 129, 1)',
                'rgba(59, 130, 246, 1)',
                'rgba(245, 158, 11, 1)',
                'rgba(217, 70, 239, 1)',
                'rgba(239, 68, 68, 1)'
            ],
            borderWidth: 1
        }]
    },
    options: {
        responsive: true,
        maintainAspectRatio: false,
        cutout: '65%',
        plugins: {
            legend: {
                position: 'bottom',
                labels: {
                    usePointStyle: true,
                    boxWidth: 8,
                    font: {
                        size: 11
                    }
                }
            }
        }
    }
});
</script>
```

## Example 4: Radar Chart
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-4 flex items-center text-blue-600">
        <i class="ri-radar-line text-xl mr-2"></i> Example 4: Radar Chart
    </h2>
    <p class="text-gray-600 mb-6">Skill assessment comparison between teams</p>
    
    <div class="flex flex-col md:flex-row">
        <div class="md:w-2/3">
            <div class="h-80">
                <canvas id="radarChart"></canvas>
            </div>
        </div>
        <div class="md:w-1/3 flex flex-col justify-center mt-6 md:mt-0 md:pl-6">
            <div class="mb-3">
                <div class="flex items-center">
                    <div class="w-4 h-4 bg-blue-500 rounded-sm mr-2"></div>
                    <span class="text-sm font-medium text-gray-700">Team Alpha</span>
                </div>
                <p class="text-xs text-gray-500 ml-6">Strongest in communication</p>
            </div>
            <div class="mb-3">
                <div class="flex items-center">
                    <div class="w-4 h-4 bg-purple-500 rounded-sm mr-2"></div>
                    <span class="text-sm font-medium text-gray-700">Team Beta</span>
                </div>
                <p class="text-xs text-gray-500 ml-6">Strongest in technical skills</p>
            </div>
        </div>
    </div>
</div>

<script>
// Radar Chart
const radarCtx = document.getElementById('radarChart').getContext('2d');
const radarChart = new Chart(radarCtx, {
    type: 'radar',
    data: {
        labels: [
            'Technical Skills',
            'Communication',
            'Teamwork',
            'Problem Solving',
            'Creativity',
            'Leadership'
        ],
        datasets: [
            {
                label: 'Team Alpha',
                data: [65, 90, 75, 70, 65, 80],
                backgroundColor: 'rgba(59, 130, 246, 0.2)',
                borderColor: 'rgba(59, 130, 246, 1)',
                pointBackgroundColor: 'rgba(59, 130, 246, 1)',
                borderWidth: 2
            },
            {
                label: 'Team Beta',
                data: [85, 70, 65, 75, 60, 65],
                backgroundColor: 'rgba(139, 92, 246, 0.2)',
                borderColor: 'rgba(139, 92, 246, 1)',
                pointBackgroundColor: 'rgba(139, 92, 246, 1)',
                borderWidth: 2
            }
        ]
    },
    options: {
        responsive: true,
        maintainAspectRatio: false,
        scales: {
            r: {
                angleLines: {
                    color: 'rgba(229, 231, 235, 0.7)'
                },
                grid: {
                    color: 'rgba(229, 231, 235, 0.5)'
                },
                pointLabels: {
                    font: {
                        size: 11
                    }
                },
                suggestedMin: 0,
                suggestedMax: 100
            }
        },
        plugins: {
            legend: {
                display: false
            }
        }
    }
});
</script>
```

## Example 5: Mixed Chart with Stats
```html
<div class="mb-16 bg-white p-8 rounded-lg shadow-md">
    <h2 class="text-xl font-semibold mb-6 flex items-center text-blue-600">
        <i class="ri-bar-chart-grouped-line text-xl mr-2"></i> Example 5: Mixed Chart with Stats
    </h2>
    
    <!-- Stats Cards -->
    <div class="grid grid-cols-2 md:grid-cols-4 gap-4 mb-6">
        <div class="bg-blue-50 p-4 rounded-lg border border-blue-100">
            <div class="text-blue-600 mb-1">
                <i class="ri-user-line text-lg"></i>
            </div>
            <p class="text-2xl font-bold text-gray-800">1,243</p>
            <p class="text-sm text-gray-500">Total Users</p>
            <div class="mt-1 text-xs text-green-600 flex items-center">
                <i class="ri-arrow-up-s-line"></i>
                <span>12.5% increase</span>
            </div>
        </div>
        
        <div class="bg-green-50 p-4 rounded-lg border border-green-100">
            <div class="text-green-600 mb-1">
                <i class="ri-shopping-cart-line text-lg"></i>
            </div>
            <p class="text-2xl font-bold text-gray-800">$12,543</p>
            <p class="text-sm text-gray-500">Total Revenue</p>
            <div class="mt-1 text-xs text-green-600 flex items-center">
                <i class="ri-arrow-up-s-line"></i>
                <span>8.2% increase</span>
            </div>
        </div>
    </div>
    
    <!-- Mixed Chart -->
    <div>
        <canvas id="mixedChart" class="w-full"></canvas>
    </div>
</div>

<script>
// Mixed Chart
const mixedCtx = document.getElementById('mixedChart').getContext('2d');
const mixedChart = new Chart(mixedCtx, {
    type: 'bar',
    data: {
        labels: ['Jan', 'Feb', 'Mar', 'Apr', 'May', 'Jun'],
        datasets: [
            {
                type: 'line',
                label: 'Average Order Value',
                data: [68, 72, 73, 80, 76, 85],
                borderColor: 'rgb(75, 85, 99)',
                backgroundColor: 'rgba(75, 85, 99, 0.5)',
                borderWidth: 2,
                tension: 0.2,
                yAxisID: 'y1'
            },
            {
                type: 'bar',
                label: 'Revenue',
                data: [15000, 17000, 16500, 19000, 18000, 22000],
                backgroundColor: 'rgba(59, 130, 246, 0.7)',
                borderColor: 'rgba(59, 130, 246, 1)',
                borderWidth: 1,
                yAxisID: 'y'
            },
            {
                type: 'bar',
                label: 'Cost',
                data: [9000, 10200, 9900, 11400, 10800, 13200],
                backgroundColor: 'rgba(107, 114, 128, 0.7)',
                borderColor: 'rgba(107, 114, 128, 1)',
                borderWidth: 1,
                yAxisID: 'y'
            }
        ]
    },
    options: {
        responsive: true,
        maintainAspectRatio: false,
        scales: {
            y: {
                beginAtZero: true,
                position: 'left',
                title: {
                    display: true,
                    text: 'Revenue / Cost ($)',
                    font: {
                        size: 12
                    }
                },
                grid: {
                    color: 'rgba(229, 231, 235, 0.5)'
                }
            },
            y1: {
                beginAtZero: true,
                position: 'right',
                title: {
                    display: true,
                    text: 'Average Order ($)',
                    font: {
                        size: 12
                    }
                },
                grid: {
                    drawOnChartArea: false
                }
            },
            x: {
                grid: {
                    display: false
                }
            }
        },
        plugins: {
            legend: {
                position: 'top',
                labels: {
                    usePointStyle: true,
                    boxWidth: 8
                }
            }
        }
    }
});
</script>
```
