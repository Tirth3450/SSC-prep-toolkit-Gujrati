# SSC-prep-toolkit-Gujrati
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Exam Prep Toolkit</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <style>
        .question-card {
            transition: all 0.3s ease;
        }
        .question-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
        }
        .option-selected {
            background-color: #3b82f6;
            color: white;
        }
    </style>
</head>
<body class="bg-gray-50 min-h-screen">
    <!-- Header -->
    <header class="bg-blue-600 text-white py-4 shadow-lg">
        <div class="container mx-auto px-4 flex justify-between items-center">
            <h1 class="text-2xl font-bold">કેન્દ્રીય પરીક્ષા તૈયારી</h1>
            <div class="flex space-x-4">
                <button class="bg-blue-700 px-4 py-2 rounded-lg">પ્રવેશ કરો</button>
            </div>
        </div>
    </header>

    <!-- Main Content -->
    <main class="container mx-auto px-4 py-8">
        <!-- Exam Selection -->
        <section class="mb-12">
            <h2 class="text-2xl font-bold mb-6">તમારી પરીક્ષા પસંદ કરો</h2>
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow-md p-6 question-card cursor-pointer">
                    <div class="flex items-center mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/eb689891-fc59-47e3-b7fb-9e9a8b1de42f.png" alt="SSC logo with blue background" class="mr-3">
                        <h3 class="font-semibold text-lg">SSC-GPSC</h3>
                    </div>
                    <p class="text-gray-600 mb-4">ગુજરાતી માધ્યમ • પ્રશ્નપત્રો • મોક ટેસ્ટ</p>
                    <button class="bg-blue-600 text-white px-4 py-2 rounded-lg w-full">તૈયારી શરૂ કરો</button>
                </div>

                <div class="bg-white rounded-xl shadow-md p-6 question-card cursor-pointer">
                    <div class="flex items-center mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/7ea7da14-13cb-4fb2-b0f5-46471aed5984.png" alt="Banking exam logo with green background" class="mr-3">
                        <h3 class="font-semibold text-lg">Banking Exams</h3>
                    </div>
                    <p class="text-gray-600 mb-4">IBPS • SBI • RBI • Mock Tests</p>
                    <button class="bg-blue-600 text-white px-4 py-2 rounded-lg w-full">Start Preparation</button>
                </div>

                <div class="bg-white rounded-xl shadow-md p-6 question-card cursor-pointer">
                    <div class="flex items-center mb-4">
                        <img src="https://storage.googleapis.com/workspace-0f70711f-8b4e-4d94-86f1-2a93ccde5887/image/13fdf18d-8b73-4579-b129-454028977dc8.png" alt="State exams logo with orange background" class="mr-3">
                        <h3 class="font-semibold text-lg">State Level Exams</h3>
                    </div>
                    <p class="text-gray-600 mb-4">State PSC • Police • Teacher Exams</p>
                    <button class="bg-blue-600 text-white px-4 py-2 rounded-lg w-full">Start Preparation</button>
                </div>
            </div>
        </section>

        <!-- Sample Test Section -->
        <section class="mb-12">
            <h2 class="text-2xl font-bold mb-6">નમૂના પ્રશ્નો ચકાસો</h2>
            
            <!-- Question 1 -->
            <div class="bg-white rounded-xl shadow-md p-6 mb-6">
                <div class="flex justify-between items-center mb-4">
                    <p class="text-gray-500">Quantitative Aptitude</p>
                    <span class="bg-blue-100 text-blue-800 px-3 py-1 rounded-full text-sm">Difficulty: Medium</span>
                </div>
                <p class="font-medium mb-4">If the ratio of the areas of two squares is 9:1, then the ratio of their perimeters is:</p>
                
                <div class="space-y-3">
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">3:1</div>
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">9:1</div>
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">6:1</div>
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">12:1</div>
                </div>
                
                <button class="mt-4 bg-blue-600 text-white px-4 py-2 rounded-lg" onclick="checkAnswer()">જવાબ તપાસો</button>
                <div id="answer-feedback" class="hidden mt-3 p-3 rounded-lg"></div>
            </div>

            <!-- Question 2 -->
            <div class="bg-white rounded-xl shadow-md p-6">
                <div class="flex justify-between items-center mb-4">
                    <p class="text-gray-500">General Awareness</p>
                    <span class="bg-green-100 text-green-800 px-3 py-1 rounded-full text-sm">Difficulty: Easy</span>
                </div>
                <p class="font-medium mb-4">The Indian Space Research Organisation (ISRO) headquarters is located at:</p>
                
                <div class="space-y-3">
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">New Delhi</div>
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">Mumbai</div>
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">Bengaluru</div>
                    <div class="option px-4 py-3 border rounded-lg cursor-pointer" onclick="selectOption(this)">Chennai</div>
                </div>
                
                <button class="mt-4 bg-blue-600 text-white px-4 py-2 rounded-lg" onclick="checkAnswer()">Check Answer</button>
                <div id="answer-feedback-2" class="hidden mt-3 p-3 rounded-lg"></div>
            </div>
        </section>

        <!-- Features Section -->
        <section class="mb-12">
            <h2 class="text-2xl font-bold mb-6">Key Features</h2>
            
            <div class="grid grid-cols-1 md:grid-cols-3 gap-6">
                <div class="bg-white rounded-xl shadow-md p-6">
                    <div class="flex items-center mb-4">
                        <div class="bg-blue-100 p-3 rounded-full mr-4">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-blue-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9 5H7a2 2 0 00-2 2v12a2 2 0 002 2h10a2 2 0 002-2V7a2 2 0 00-2-2h-2M9 5a2 2 0 002 2h2a2 2 0 002-2M9 5a2 2 0 012-2h2a2 2 0 012 2" />
                            </svg>
                        </div>
                        <h3 class="font-semibold">Previous Year Papers</h3>
                    </div>
                    <p class="text-gray-600">Access solved papers from last 5 years with detailed solutions</p>
                </div>

                <div class="bg-white rounded-xl shadow-md p-6">
                    <div class="flex items-center mb-4">
                        <div class="bg-green-100 p-3 rounded-full mr-4">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-green-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M9.663 17h4.673M12 3v1m6.364 1.636l-.707.707M21 12h-1M4 12H3m3.343-5.657l-.707-.707m2.828 9.9a5 5 0 117.072 0l-.548.547A3.374 3.374 0 0014 18.469V19a2 2 0 11-4 0v-.531c0-.895-.356-1.754-.988-2.386l-.548-.547z" />
                            </svg>
                        </div>
                        <h3 class="font-semibold">Smart Analysis</h3>
                    </div>
                    <p class="text-gray-600">Get detailed performance reports and improvement suggestions</p>
                </div>

                <div class="bg-white rounded-xl shadow-md p-6">
                    <div class="flex items-center mb-4">
                        <div class="bg-purple-100 p-3 rounded-full mr-4">
                            <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 text-purple-600" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 7V3m8 4V3m-9 8h10M5 21h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v12a2 2 0 002 2z" />
                            </svg>
                        </div>
                        <h3 class="font-semibold">Daily Targets</h3>
                    </div>
                    <p class="text-gray-600">Personalized study plans based on your exam date and syllabus</p>
                </div>
            </div>
        </section>
    </main>

    <!-- Footer -->
    <footer class="bg-gray-800 text-white py-8">
        <div class="container mx-auto px-4">
            <div class="grid grid-cols-1 md:grid-cols-4 gap-8">
                <div>
                    <h3 class="font-bold text-lg mb-4">ExamPrep Toolkit</h3>
                    <p class="text-gray-400">ગુજરાતી વિદ્યાર્થીઓ માટે કેન્દ્રીય પરીક્ષાઓની તૈયારી</p>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Exams</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li>SSC Exams</li>
                        <li>Banking Exams</li>
                        <li>Railway Exams</li>
                        <li>Defense Exams</li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Resources</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li>Mock Tests</li>
                        <li>Previous Papers</li>
                        <li>Video Lessons</li>
                        <li>Study Notes</li>
                    </ul>
                </div>
                <div>
                    <h4 class="font-semibold mb-4">Contact</h4>
                    <ul class="space-y-2 text-gray-400">
                        <li>support@examprep.com</li>
                        <li>+91 9876543210</li>
                        <li>Feedback</li>
                    </ul>
                </div>
            </div>
            <div class="border-t border-gray-700 mt-8 pt-6 text-center text-gray-400">
                <p>© 2025 ExamPrep Toolkit. All rights reserved.</p>
            </div>
        </div>
    </footer>

    <script>
        function selectOption(option) {
            // Remove selected class from all options
            const options = document.querySelectorAll('.option');
            options.forEach(opt => opt.classList.remove('option-selected'));
            
            // Add selected class to clicked option
            option.classList.add('option-selected');
        }

        function checkAnswer() {
            const selectedOption = document.querySelector('.option-selected');
            if (!selectedOption) {
                alert('Please select an answer first!');
                return;
            }

            const feedbackDiv = document.getElementById('answer-feedback');
            const answer = selectedOption.textContent.trim();
            
            // For demo purposes - correct answers are hardcoded
            if (answer === '3:1') {
                feedbackDiv.textContent = 'Correct! The ratio of perimeters of squares is equal to the square root of the ratio of their areas.';
                feedbackDiv.className = 'bg-green-100 text-green-800 mt-3 p-3 rounded-lg';
            } else if (answer === 'Bengaluru') {
                feedbackDiv.textContent = 'Correct! ISRO headquarters is located in Bengaluru (formerly Bangalore).';
                feedbackDiv.className = 'bg-green-100 text-green-800 mt-3 p-3 rounded-lg';
            } else {
                feedbackDiv.textContent = 'Incorrect. Try again!';
                feedbackDiv.className = 'bg-red-100 text-red-800 mt-3 p-3 rounded-lg';
            }
            
            feedbackDiv.classList.remove('hidden');
        }
    </script>
</body>
</html>
