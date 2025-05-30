```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Quiz - 4 Etapas</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://cdn.jsdelivr.net/npm/remixicon@3.5.0/fonts/remixicon.css" rel="stylesheet">
</head>
<body class="bg-gradient-to-br from-blue-50 to-indigo-100 min-h-screen">
    <div class="container mx-auto px-4 py-8">
        <!-- Header -->
        <div class="text-center mb-8">
            <h1 class="text-4xl font-bold text-gray-800 mb-2">Quiz Interativo</h1>
            <p class="text-gray-600">Complete as 4 etapas do quiz</p>
        </div>

        <!-- Progress Bar -->
        <div class="max-w-2xl mx-auto mb-8">
            <div class="flex items-center justify-between mb-4">
                <span class="text-sm font-medium text-gray-600">Progresso</span>
                <span id="progress-text" class="text-sm font-medium text-indigo-600">1 de 4</span>
            </div>
            <div class="w-full bg-gray-200 rounded-full h-2">
                <div id="progress-bar" class="bg-indigo-600 h-2 rounded-full transition-all duration-300" style="width: 25%"></div>
            </div>
        </div>

        <!-- Quiz Container -->
        <div class="max-w-2xl mx-auto bg-white rounded-2xl shadow-xl overflow-hidden">
            <!-- Step 1 -->
            <div id="step-1" class="quiz-step p-8">
                <div class="flex items-center mb-6">
                    <div class="bg-indigo-100 p-3 rounded-full mr-4">
                        <i class="ri-questionnaire-line text-2xl text-indigo-600"></i>
                    </div>
                    <h2 class="text-2xl font-bold text-gray-800">Etapa 1</h2>
                </div>
                <h3 class="text-xl font-semibold text-gray-700 mb-6">Qual é a capital do Brasil?</h3>
                <div class="space-y-3">
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-indigo-300 transition-colors">
                        <input type="radio" name="q1" value="a" class="mr-3 text-indigo-600">
                        <span class="text-gray-700">São Paulo</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-indigo-300 transition-colors">
                        <input type="radio" name="q1" value="b" class="mr-3 text-indigo-600">
                        <span class="text-gray-700">Rio de Janeiro</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-indigo-300 transition-colors">
                        <input type="radio" name="q1" value="c" class="mr-3 text-indigo-600">
                        <span class="text-gray-700">Brasília</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-indigo-300 transition-colors">
                        <input type="radio" name="q1" value="d" class="mr-3 text-indigo-600">
                        <span class="text-gray-700">Salvador</span>
                    </label>
                </div>
            </div>

            <!-- Step 2 -->
            <div id="step-2" class="quiz-step p-8 hidden">
                <div class="flex items-center mb-6">
                    <div class="bg-green-100 p-3 rounded-full mr-4">
                        <i class="ri-earth-line text-2xl text-green-600"></i>
                    </div>
                    <h2 class="text-2xl font-bold text-gray-800">Etapa 2</h2>
                </div>
                <h3 class="text-xl font-semibold text-gray-700 mb-6">Qual o maior planeta do Sistema Solar?</h3>
                <div class="space-y-3">
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-green-300 transition-colors">
                        <input type="radio" name="q2" value="a" class="mr-3 text-green-600">
                        <span class="text-gray-700">Terra</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-green-300 transition-colors">
                        <input type="radio" name="q2" value="b" class="mr-3 text-green-600">
                        <span class="text-gray-700">Júpiter</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-green-300 transition-colors">
                        <input type="radio" name="q2" value="c" class="mr-3 text-green-600">
                        <span class="text-gray-700">Saturno</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-green-300 transition-colors">
                        <input type="radio" name="q2" value="d" class="mr-3 text-green-600">
                        <span class="text-gray-700">Marte</span>
                    </label>
                </div>
            </div>

            <!-- Step 3 -->
            <div id="step-3" class="quiz-step p-8 hidden">
                <div class="flex items-center mb-6">
                    <div class="bg-purple-100 p-3 rounded-full mr-4">
                        <i class="ri-calculator-line text-2xl text-purple-600"></i>
                    </div>
                    <h2 class="text-2xl font-bold text-gray-800">Etapa 3</h2>
                </div>
                <h3 class="text-xl font-semibold text-gray-700 mb-6">Quanto é 15 × 8?</h3>
                <div class="space-y-3">
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-purple-300 transition-colors">
                        <input type="radio" name="q3" value="a" class="mr-3 text-purple-600">
                        <span class="text-gray-700">120</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-purple-300 transition-colors">
                        <input type="radio" name="q3" value="b" class="mr-3 text-purple-600">
                        <span class="text-gray-700">110</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-purple-300 transition-colors">
                        <input type="radio" name="q3" value="c" class="mr-3 text-purple-600">
                        <span class="text-gray-700">130</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-purple-300 transition-colors">
                        <input type="radio" name="q3" value="d" class="mr-3 text-purple-600">
                        <span class="text-gray-700">125</span>
                    </label>
                </div>
            </div>

            <!-- Step 4 -->
            <div id="step-4" class="quiz-step p-8 hidden">
                <div class="flex items-center mb-6">
                    <div class="bg-orange-100 p-3 rounded-full mr-4">
                        <i class="ri-book-line text-2xl text-orange-600"></i>
                    </div>
                    <h2 class="text-2xl font-bold text-gray-800">Etapa 4</h2>
                </div>
                <h3 class="text-xl font-semibold text-gray-700 mb-6">Quem escreveu "Dom Casmurro"?</h3>
                <div class="space-y-3">
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-orange-300 transition-colors">
                        <input type="radio" name="q4" value="a" class="mr-3 text-orange-600">
                        <span class="text-gray-700">José de Alencar</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-orange-300 transition-colors">
                        <input type="radio" name="q4" value="b" class="mr-3 text-orange-600">
                        <span class="text-gray-700">Machado de Assis</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-orange-300 transition-colors">
                        <input type="radio" name="q4" value="c" class="mr-3 text-orange-600">
                        <span class="text-gray-700">Clarice Lispector</span>
                    </label>
                    <label class="flex items-center p-4 border-2 border-gray-200 rounded-lg cursor-pointer hover:border-orange-300 transition-colors">
                        <input type="radio" name="q4" value="d" class="mr-3 text-orange-600">
                        <span class="text-gray-700">Graciliano Ramos</span>
                    </label>
                </div>
            </div>

            <!-- Results -->
            <div id="results" class="p-8 hidden text-center">
                <div class="bg-green-100 p-6 rounded-full w-24 h-24 mx-auto mb-6 flex items-center justify-center">
                    <i class="ri-trophy-line text-4xl text-green-600"></i>
                </div>
                <h2 class="text-3xl font-bold text-gray-800 mb-4">Quiz Concluído!</h2>
                <p class="text-xl text-gray-600 mb-6">Sua pontuação:</p>
                <div id="score" class="text-5xl font-bold text-indigo-600 mb-8">0/4</div>
                <button onclick="restartQuiz()" class="bg-indigo-600 text-white px-8 py-3 rounded-lg font-semibold hover:bg-indigo-700 transition-colors">
                    <i class="ri-restart-line mr-2"></i>
                    Refazer Quiz
                </button>
            </div>

            <!-- Navigation - Only Previous Button -->
            <div id="navigation" class="bg-gray-50 px-8 py-4 flex justify-between items-center">
                <button id="prev-btn" onclick="previousStep()" class="bg-gray-500 text-white px-6 py-2 rounded-lg font-semibold hover:bg-gray-600 transition-colors disabled:opacity-50 disabled:cursor-not-allowed" disabled>
                    <i class="ri-arrow-left-line mr-2"></i>
                    Anterior
                </button>
                <div class="text-sm text-gray-500">
                    <i class="ri-information-line mr-1"></i>
                    Clique em uma resposta para avançar
                </div>
            </div>
        </div>
    </div>

    <script>
        let currentStep = 1;
        const totalSteps = 4;
        const answers = {};
        const correctAnswers = { q1: 'c', q2: 'b', q3: 'a', q4: 'b' };

        function updateProgress() {
            const progress = (currentStep / totalSteps) * 100;
            document.getElementById('progress-bar').style.width = progress + '%';
            document.getElementById('progress-text').textContent = `${currentStep} de ${totalSteps}`;
        }

        function showStep(step) {
            // Hide all steps
            document.querySelectorAll('.quiz-step').forEach(el => el.classList.add('hidden'));
            document.getElementById('results').classList.add('hidden');
            document.getElementById('navigation').classList.remove('hidden');
            
            if (step <= totalSteps) {
                document.getElementById(`step-${step}`).classList.remove('hidden');
                updateProgress();
            } else {
                showResults();
            }
            
            updateNavigationButtons();
        }

        function updateNavigationButtons() {
            const prevBtn = document.getElementById('prev-btn');
            prevBtn.disabled = currentStep === 1;
        }

        function nextStep() {
            // Auto-advance when answer is selected
            const currentQuestion = `q${currentStep}`;
            const selectedAnswer = document.querySelector(`input[name="${currentQuestion}"]:checked`);
            
            if (selectedAnswer) {
                answers[currentQuestion] = selectedAnswer.value;
                
                // Add a small delay for better UX
                setTimeout(() => {
                    if (currentStep < totalSteps) {
                        currentStep++;
                        showStep(currentStep);
                    } else {
                        currentStep++;
                        showStep(currentStep);
                    }
                }, 300);
            }
        }

        function previousStep() {
            if (currentStep > 1) {
                currentStep--;
                showStep(currentStep);
                
                // Restore previous selection
                const prevQuestion = `q${currentStep}`;
                if (answers[prevQuestion]) {
                    const prevInput = document.querySelector(`input[name="${prevQuestion}"][value="${answers[prevQuestion]}"]`);
                    if (prevInput) {
                        prevInput.checked = true;
                        // Trigger styling update
                        prevInput.dispatchEvent(new Event('change'));
                    }
                }
            }
        }

        function showResults() {
            document.getElementById('results').classList.remove('hidden');
            document.getElementById('navigation').classList.add('hidden');
            
            let score = 0;
            for (let question in correctAnswers) {
                if (answers[question] === correctAnswers[question]) {
                    score++;
                }
            }
            
            document.getElementById('score').textContent = `${score}/${totalSteps}`;
            
            // Update progress to 100%
            document.getElementById('progress-bar').style.width = '100%';
            document.getElementById('progress-text').textContent = 'Concluído';
        }

        function restartQuiz() {
            currentStep = 1;
            Object.keys(answers).forEach(key => delete answers[key]);
            
            // Clear all radio buttons and styling
            document.querySelectorAll('input[type="radio"]').forEach(input => {
                input.checked = false;
            });
            
            // Clear all selection styling
            document.querySelectorAll('label').forEach(label => {
                label.classList.remove('border-indigo-500', 'border-green-500', 'border-purple-500', 'border-orange-500', 'bg-indigo-50', 'bg-green-50', 'bg-purple-50', 'bg-orange-50');
            });
            
            showStep(1);
        }

        // Initialize quiz
        showStep(1);

        // Add event listeners to radio buttons for auto-advance
        document.querySelectorAll('input[type="radio"]').forEach(input => {
            input.addEventListener('change', function() {
                // Remove previous selection styling from all labels in current step
                this.closest('.quiz-step').querySelectorAll('label').forEach(label => {
                    label.classList.remove('border-indigo-500', 'border-green-500', 'border-purple-500', 'border-orange-500', 'bg-indigo-50', 'bg-green-50', 'bg-purple-50', 'bg-orange-50');
                });
                
                // Add selection styling based on current step
                const colors = {
                    1: ['border-indigo-500', 'bg-indigo-50'],
                    2: ['border-green-500', 'bg-green-50'],
                    3: ['border-purple-500', 'bg-purple-50'],
                    4: ['border-orange-500', 'bg-orange-50']
                };
                
                this.closest('label').classList.add(...colors[currentStep]);
                
                // Auto-advance to next step
                nextStep();
            });
        });
    </script>
</body>
</html>
```
