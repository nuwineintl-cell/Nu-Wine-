```
skillbuddy-ai/
├── css/
├── js/
└── assets/
    ├── images/
    └── audio/
```

📄 FILE 1: index.html (Main File)

Save this in the main skillbuddy-ai folder:

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>SkillBuddy Nigeria 🤖 - AI-Powered Learning</title>
    <link rel="stylesheet" href="css/style.css">
</head>
<body>
    <div class="container">
        <!-- WELCOME SCREEN -->
        <div id="welcome-screen" class="screen active">
            <div class="header">
                <div class="ai-badge">🤖 AI Powered</div>
                <div class="logo">🎯</div>
                <div class="title">SkillBuddy Nigeria</div>
                <div class="subtitle">AI-Powered Skill Learning</div>
            </div>
            <div class="content">
                <div class="ai-feature-card">
                    <strong>🚀 AI Features Included:</strong>
                    <div class="feature-list">
                        • Personalized Learning Path<br>
                        • AI Tutor Chat Support<br>
                        • Adaptive Difficulty<br>
                        • Progress Analytics<br>
                        • Smart Recommendations
                    </div>
                </div>
                
                <button class="btn btn-primary" onclick="app.showScreen('signup-screen')">
                    Start AI-Powered Learning
                </button>
                
                <button class="btn btn-secondary" onclick="app.showScreen('login-screen')">
                    I Have an Account
                </button>
                
                <div class="footer-note">
                    🤖 AI Tutor • 📊 Smart Analytics • 🎯 Personalized
                </div>
            </div>
        </div>

        <!-- SIGNUP SCREEN -->
        <div id="signup-screen" class="screen">
            <div class="header">
                <div class="title">AI Learning Profile</div>
                <div class="subtitle">Tell us about your goals</div>
            </div>
            <div class="content">
                <input type="text" id="user-name" class="form-input" placeholder="Your Name" value="Test User">
                <input type="tel" id="user-phone" class="form-input" placeholder="Phone Number" value="09121468809">
                
                <div class="form-section">
                    <strong>Choose Your Skill:</strong>
                    <div class="skill-grid">
                        <div class="skill-btn" onclick="app.selectSkill('piano')">🎹 Piano</div>
                        <div class="skill-btn" onclick="app.selectSkill('design')">🎨 Design</div>
                        <div class="skill-btn" onclick="app.selectSkill('drums')">🥁 Drums</div>
                        <div class="skill-btn" onclick="app.selectSkill('violin')">🎻 Violin</div>
                        <div class="skill-btn" onclick="app.selectSkill('voice')">🎤 Voice Training</div>
                        <div class="skill-btn" onclick="app.selectSkill('karate')">🥋 Karate</div>
                    </div>
                </div>
                
                <div class="form-section">
                    <strong>Learning Goal:</strong>
                    <select id="learning-goal" class="form-select">
                        <option value="hobby">🎯 For Fun & Hobby</option>
                        <option value="career">💼 For Career Development</option>
                        <option value="performance">🎭 For Live Performance</option>
                        <option value="business">💼 For Business Use</option>
                    </select>
                </div>
                
                <div class="form-section">
                    <strong>Available Practice Time:</strong>
                    <select id="practice-time" class="form-select">
                        <option value="15">15 minutes daily</option>
                        <option value="30">30 minutes daily</option>
                        <option value="45">45 minutes daily</option>
                        <option value="60">1 hour daily</option>
                    </select>
                </div>
                
                <button class="btn btn-primary" onclick="app.createAILearningProfile()">
                    🤖 Create AI Learning Plan
                </button>
                
                <button class="btn btn-secondary" onclick="app.showScreen('welcome-screen')">
                    Back
                </button>
            </div>
        </div>

        <!-- DASHBOARD SCREEN -->
        <div id="dashboard-screen" class="screen">
            <div class="header">
                <div class="title" id="greeting">Hello, User!</div>
                <div class="subtitle" id="user-skill">AI Learning Active</div>
            </div>
            <div class="content">
                <!-- AI Recommendations -->
                <div class="ai-recommendation" id="ai-recommendation">
                    <strong>🤖 AI Suggestion:</strong>
                    <div id="recommendation-text">Based on your progress, I recommend focusing on chord transitions today.</div>
                </div>
                
                <!-- Adaptive Difficulty -->
                <div class="adaptive-difficulty">
                    <strong>🎯 Current Level: <span id="difficulty-level">Beginner</span></strong>
                    <div class="difficulty-subtext">
                        AI-adjusted based on your performance
                    </div>
                </div>
                
                <div class="lesson-card">
                    <strong>📚 AI-Personalized Lesson</strong>
                    <div id="lesson-title">Piano Basics - Hand Positioning</div>
                    <div class="lesson-meta">
                        ⏱️ <span id="lesson-duration">15 minutes</span> • 
                        🎯 <span id="lesson-focus">Fundamentals</span>
                    </div>
                    <button class="btn btn-primary" onclick="app.startAILesson()">
                        Start AI Lesson
                    </button>
                </div>
                
                <!-- Progress Analytics -->
                <div class="analytics-card">
                    <strong>📊 AI Progress Analytics</strong>
                    <div class="analytics-grid">
                        <div class="analytics-item">
                            <div class="analytics-value" id="completion-rate">85%</div>
                            <div class="analytics-label">Success Rate</div>
                        </div>
                        <div class="analytics-item">
                            <div class="analytics-value" id="improvement-score">+12%</div>
                            <div class="analytics-label">Weekly Improvement</div>
                        </div>
                        <div class="analytics-item">
                            <div class="analytics-value" id="consistency-score">94%</div>
                            <div class="analytics-label">Consistency</div>
                        </div>
                    </div>
                </div>
                
                <button class="btn btn-ai" onclick="app.showScreen('ai-tutor-screen')">
                    🧠 Talk to AI Tutor
                </button>

                <button class="btn btn-ai" onclick="app.showScreen('voice-training-screen')">
                    🎤 Start Voice Training
                </button>
                
                <button class="btn btn-secondary" onclick="app.showPayment()">
                    💳 Upgrade to Premium
                </button>
            </div>
        </div>

        <!-- AI TUTOR CHAT SCREEN -->
        <div id="ai-tutor-screen" class="screen">
            <div class="header">
                <div class="title">🧠 AI Tutor</div>
                <div class="subtitle">Ask me anything about your skill!</div>
            </div>
            <div class="content">
                <div class="ai-chat" id="chat-messages">
                    <div class="message ai-message">
                        Hello! I'm your AI tutor. I can help you with:
                        • Lesson explanations
                        • Practice techniques  
                        • Problem solving
                        • Progress advice
                        What would you like to know?
                    </div>
                </div>
                
                <div class="typing-indicator" id="typing-indicator">
                    AI Tutor is typing...
                </div>
                
                <div class="chat-input">
                    <input type="text" id="chat-input" placeholder="Ask your question..." onkeypress="app.handleChatInput(event)">
                    <button class="btn btn-primary" onclick="app.sendMessage()">Send</button>
                </div>
                
                <div class="quick-questions">
                    <strong>Quick Questions:</strong>
                    <div class="quick-buttons">
                        <button class="btn quick-btn" onclick="app.askQuickQuestion('How can I improve my rhythm?')">Improve rhythm</button>
                        <button class="btn quick-btn" onclick="app.askQuickQuestion('Explain this lesson again')">Explain lesson</button>
                        <button class="btn quick-btn" onclick="app.askQuickQuestion('Give me practice exercises')">Practice exercises</button>
                    </div>
                </div>
                
                <button class="btn btn-secondary" onclick="app.showScreen('dashboard-screen')">
                    ← Back to Dashboard
                </button>
            </div>
        </div>

        <!-- LESSON SCREEN -->
        <div id="lesson-screen" class="screen">
            <div class="header">
                <div class="title" id="lesson-screen-title">AI Lesson</div>
                <div class="subtitle">Personalized for you</div>
            </div>
            <div class="content">
                <div id="lesson-content">
                    <!-- AI-generated lesson content will go here -->
                </div>
                
                <button class="btn btn-primary" onclick="app.completeAILesson()">
                    ✅ Complete Lesson
                </button>
                
                <button class="btn btn-ai" onclick="app.showScreen('ai-tutor-screen')">
                    🧠 Ask AI Tutor
                </button>
                
                <button class="btn btn-secondary" onclick="app.showScreen('dashboard-screen')">
                    ← Back to Dashboard
                </button>
            </div>
        </div>

        <!-- VOICE TRAINING SCREEN -->
        <div id="voice-training-screen" class="screen">
            <div class="header">
                <div class="title">🎤 Voice Training</div>
                <div class="subtitle">AI-Powered Vocal Development</div>
            </div>
            <div class="content">
                <!-- Voice Level Selection -->
                <div class="level-selection">
                    <strong>Select Your Vocal Level:</strong>
                    <div class="level-grid">
                        <div class="level-btn" onclick="voiceTraining.selectLevel('beginner')">
                            🐣 Beginner
                            <div class="level-desc">Just starting out</div>
                        </div>
                        <div class="level-btn" onclick="voiceTraining.selectLevel('intermediate')">
                            🚀 Intermediate
                            <div class="level-desc">Some experience</div>
                        </div>
                        <div class="level-btn" onclick="voiceTraining.selectLevel('advanced')">
                            ⚡ Advanced
                            <div class="level-desc">Regular performer</div>
                        </div>
                        <div class="level-btn" onclick="voiceTraining.selectLevel('professional')">
                            🏆 Professional
                            <div class="level-desc">Stage experience</div>
                        </div>
                    </div>
                </div>

                <!-- Daily Voice Exercise -->
                <div class="voice-exercise-card" id="voice-exercise-card">
                    <div class="exercise-header">
                        <strong>📅 Today's Vocal Exercise</strong>
                        <div class="exercise-difficulty" id="exercise-difficulty">Beginner</div>
                    </div>
                    <div class="exercise-content">
                        <div id="current-exercise">Lip trills for 2 minutes</div>
                        <div class="exercise-timer">
                            <div class="timer-display" id="timer-display">02:00</div>
                            <button class="btn btn-primary" onclick="voiceTraining.startExercise()" id="start-exercise-btn">
                                Start Exercise
                            </button>
                            <button class="btn btn-secondary" onclick="voiceTraining.stopExercise()" id="stop-exercise-btn" style="display: none;">
                                Stop Exercise
                            </button>
                        </div>
                    </div>
                </div>

                <!-- Posture Guide -->
                <div class="posture-guide">
                    <strong>🧘 Proper Singing Posture</strong>
                    <div class="posture-steps">
                        <div class="posture-step">
                            <span class="step-number">1</span>
                            <span>Feet shoulder-width apart</span>
                        </div>
                        <div class="posture-step">
                            <span class="step-number">2</span>
                            <span>Knees slightly bent</span>
                        </div>
                        <div class="posture-step">
                            <span class="step-number">3</span>
                            <span>Spine straight, shoulders relaxed</span>
                        </div>
                        <div class="posture-step">
                            <span class="step-number">4</span>
                            <span>Chin parallel to floor</span>
                        </div>
                    </div>
                    <button class="btn btn-secondary" onclick="voiceTraining.showPostureDemo()">
                        🎬 View Posture Demo
                    </button>
                </div>

                <!-- Breathing Techniques -->
                <div class="breathing-techniques">
                    <strong>🌬️ Breathing Exercises</strong>
                    <div class="breathing-exercises">
                        <div class="breathing-exercise" onclick="voiceTraining.startBreathingExercise('diaphragmatic')">
                            <strong>Diaphragmatic Breathing</strong>
                            <div>4-7-8 technique for vocal support</div>
                        </div>
                        <div class="breathing-exercise" onclick="voiceTraining.startBreathingExercise('ribcage')">
                            <strong>Ribcage Expansion</strong>
                            <div>Expand ribs without shoulder movement</div>
                        </div>
                        <div class="breathing-exercise" onclick="voiceTraining.startBreathingExercise('panting')">
                            <strong>Panting Exercise</strong>
                            <div>Build diaphragm strength</div>
                        </div>
                    </div>
                </div>

                <!-- AI Voice Analysis -->
                <div class="voice-analysis">
                    <strong>🤖 AI Voice Analysis</strong>
                    <div class="analysis-results">
                        <div class="analysis-item">
                            <div class="analysis-label">Pitch Stability</div>
                            <div class="analysis-bar">
                                <div class="analysis-fill" id="pitch-stability" style="width: 75%"></div>
                            </div>
                            <div class="analysis-value" id="pitch-value">75%</div>
                        </div>
                        <div class="analysis-item">
                            <div class="analysis-label">Breath Control</div>
                            <div class="analysis-bar">
                                <div class="analysis-fill" id="breath-control" style="width: 60%"></div>
                            </div>
                            <div class="analysis-value" id="breath-value">60%</div>
                        </div>
                        <div class="analysis-item">
                            <div class="analysis-label">Tone Quality</div>
                            <div class="analysis-bar">
                                <div class="analysis-fill" id="tone-quality" style="width: 80%"></div>
                            </div>
                            <div class="analysis-value" id="tone-value">80%</div>
                        </div>
                    </div>
                    <button class="btn btn-ai" onclick="voiceTraining.startVoiceAnalysis()">
                        🎤 Start Voice Analysis
                    </button>
                </div>

                <!-- Progress Tracking -->
                <div class="voice-progress">
                    <strong>📈 Vocal Progress</strong>
                    <div class="progress-stats">
                        <div class="progress-stat">
                            <div class="stat-value" id="vocal-range">C3-G4</div>
                            <div class="stat-label">Vocal Range</div>
                        </div>
                        <div class="progress-stat">
                            <div class="stat-value" id="practice-streak">5</div>
                            <div class="stat-label">Day Streak</div>
                        </div>
                        <div class="progress-stat">
                            <div class="stat-value" id="endurance-score">7/10</div>
                            <div class="stat-label">Endurance</div>
                        </div>
                    </div>
                </div>

                <button class="btn btn-secondary" onclick="app.showScreen('dashboard-screen')">
                    ← Back to Dashboard
                </button>
            </div>
        </div>

        <!-- BREATHING EXERCISE SCREEN -->
        <div id="breathing-exercise-screen" class="screen">
            <div class="header">
                <div class="title" id="breathing-title">Breathing Exercise</div>
                <div class="subtitle">Follow the rhythm</div>
            </div>
            <div class="content">
                <div class="breathing-animation">
                    <div class="breathing-circle" id="breathing-circle">
                        <div class="breathing-text" id="breathing-text">Breathe In</div>
                    </div>
                </div>
                <div class="breathing-timer">
                    <div class="breathing-time" id="breathing-time">04s</div>
                    <div class="breathing-phase" id="breathing-phase">Inhale</div>
                </div>
                <div class="breathing-instructions">
                    <div id="breathing-instruction">Inhale deeply through your nose for 4 seconds</div>
                </div>
                <button class="btn btn-primary" onclick="voiceTraining.stopBreathingExercise()">
                    Complete Exercise
                </button>
            </div>
        </div>

        <!-- PAYMENT SCREEN -->
        <div id="payment-screen" class="screen">
            <div class="header">
                <div class="title">Upgrade to AI Premium</div>
                <div class="subtitle">Unlock Advanced AI Features</div>
            </div>
            <div class="content">
                <div class="ai-feature-card">
                    <strong>🚀 AI Premium Includes:</strong>
                    <div class="feature-list">
                        • Advanced Personalization<br>
                        • Voice-based AI Tutor<br>
                        • Real-time Feedback<br>
                        • Detailed Analytics<br>
                        • Priority Support
                    </div>
                </div>
                
                <div class="pricing-display">
                    <div class="price">₦500/week</div>
                    <div class="price-subtext">or ₦1,500/month</div>
                </div>
                
                <div class="payment-instructions">
                    <strong>Payment Instructions:</strong><br>
                    Send ₦500 to OPay: <strong>9121468809</strong><br>
                    Then WhatsApp screenshot to <strong>09121468809</strong>
                </div>
                
                <button class="btn btn-primary" onclick="app.simulatePayment()">
                    💳 Activate AI Premium
                </button>
                
                <button class="btn btn-secondary" onclick="app.showScreen('dashboard-screen')">
                    Maybe Later
                </button>
            </div>
        </div>
    </div>

    <script src="js/app.js"></script>
    <script src="js/voice-training.js"></script>
</body>
</html>
```

📄 FILE 2: style.css (Styles)

Save this in the css folder:

```css
* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
}

body {
    background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
    min-height: 100vh;
    padding: 20px;
}

.container {
    max-width: 400px;
    margin: 0 auto;
    background: white;
    border-radius: 20px;
    overflow: hidden;
    box-shadow: 0 20px 40px rgba(0,0,0,0.1);
}

.header {
    background: #FF6B35;
    padding: 30px 20px;
    text-align: center;
    color: white;
    position: relative;
}

.ai-badge {
    position: absolute;
    top: 10px;
    right: 10px;
    background: rgba(255,255,255,0.2);
    padding: 5px 10px;
    border-radius: 15px;
    font-size: 12px;
}

.logo {
    font-size: 48px;
    margin-bottom: 10px;
}

.title {
    font-size: 24px;
    font-weight: bold;
    margin-bottom: 5px;
}

.subtitle {
    font-size: 14px;
    opacity: 0.9;
}

.content {
    padding: 20px;
    max-height: 500px;
    overflow-y: auto;
}

.screen {
    display: none;
}

.screen.active {
    display: block;
}

/* Button Styles */
.btn {
    display: block;
    width: 100%;
    padding: 15px;
    border: none;
    border-radius: 10px;
    font-size: 16px;
    font-weight: bold;
    text-align: center;
    margin: 10px 0;
    cursor: pointer;
    transition: all 0.3s;
}

.btn-primary {
    background: #FF6B35;
    color: white;
}

.btn-secondary {
    background: #f0f0f0;
    color: #333;
    border: 2px solid #ddd;
}

.btn-ai {
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
}

.btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.2);
}

.quick-btn {
    padding: 8px 12px;
    font-size: 12px;
    margin: 2px;
}

/* Form Styles */
.form-input {
    width: 100%;
    padding: 15px;
    border: 1px solid #ddd;
    border-radius: 10px;
    margin-bottom: 10px;
    font-size: 16px;
}

.form-select {
    width: 100%;
    padding: 15px;
    border: 1px solid #ddd;
    border-radius: 10px;
    margin-top: 10px;
    font-size: 16px;
}

.form-section {
    margin: 20px 0;
}

/* Skill Grid */
.skill-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
    margin: 20px 0;
}

.skill-btn {
    padding: 15px;
    border: 2px solid #ddd;
    border-radius: 10px;
    text-align: center;
    cursor: pointer;
    transition: all 0.3s;
}

.skill-btn.selected {
    border-color: #FF6B35;
    background: #FFF0EB;
}

/* Lesson Card */
.lesson-card {
    background: #f8f9fa;
    padding: 20px;
    border-radius: 10px;
    margin: 20px 0;
    border-left: 4px solid #FF6B35;
}

.lesson-meta {
    color: #666;
    font-size: 14px;
    margin: 10px 0;
}

/* AI Features */
.ai-feature-card {
    background: linear-gradient(135deg, #667eea, #764ba2);
    color: white;
    padding: 15px;
    border-radius: 10px;
    margin: 10px 0;
}

.feature-list {
    font-size: 12px;
    margin-top: 5px;
}

.ai-recommendation {
    background: #fff3cd;
    border: 1px solid #ffeaa7;
    padding: 10px;
    border-radius: 10px;
    margin: 10px 0;
}

.adaptive-difficulty {
    background: #e8f5e8;
    padding: 10px;
    border-radius: 10px;
    margin: 10px 0;
    border-left: 4px solid #4CAF50;
}

.difficulty-subtext {
    font-size: 12px;
    color: #666;
}

/* Analytics */
.analytics-card {
    background: #f8f9fa;
    padding: 15px;
    border-radius: 10px;
    margin: 15px 0;
}

.analytics-grid {
    display: flex;
    justify-content: space-between;
    margin-top: 10px;
}

.analytics-item {
    text-align: center;
}

.analytics-value {
    font-size: 20px;
    font-weight: bold;
    color: #FF6B35;
}

.analytics-label {
    font-size: 12px;
    color: #666;
    margin-top: 5px;
}

/* AI Chat */
.ai-chat {
    background: #f8f9fa;
    border-radius: 15px;
    padding: 15px;
    margin: 15px 0;
    max-height: 300px;
    overflow-y: auto;
}

.message {
    margin: 10px 0;
    padding: 10px;
    border-radius: 10px;
    max-width: 85%;
}

.user-message {
    background: #007bff;
    color: white;
    margin-left: auto;
    text-align: right;
}

.ai-message {
    background: #e9ecef;
    color: #333;
}

.typing-indicator {
    display: none;
    padding: 10px;
    color: #666;
    font-style: italic;
}

.chat-input {
    display: flex;
    gap: 10px;
    margin-top: 10px;
}

.chat-input input {
    flex: 1;
    padding: 10px;
    border: 1px solid #ddd;
    border-radius: 10px;
}

.quick-questions {
    margin-top: 15px;
}

.quick-buttons {
    display: flex;
    flex-wrap: wrap;
    gap: 5px;
    margin-top: 10px;
}

/* Payment */
.pricing-display {
    text-align: center;
    margin: 20px 0;
}

.price {
    font-size: 24px;
    font-weight: bold;
    color: #FF6B35;
}

.price-subtext {
    color: #666;
    margin: 10px 0;
}

.payment-instructions {
    background: #e8f5e8;
    padding: 15px;
    border-radius: 10px;
    margin: 20px 0;
    text-align: center;
}

/* Footer */
.footer-note {
    text-align: center;
    margin-top: 20px;
    color: #666;
    font-size: 12px;
}

/* Voice Training Specific Styles */
.level-selection {
    margin: 20px 0;
}

.level-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 10px;
    margin-top: 10px;
}

.level-btn {
    padding: 15px;
    border: 2px solid #ddd;
    border-radius: 10px;
    text-align: center;
    cursor: pointer;
    transition: all 0.3s;
}

.level-btn.selected {
    border-color: #FF6B35;
    background: #FFF0EB;
}

.level-desc {
    font-size: 12px;
    color: #666;
    margin-top: 5px;
}

.voice-exercise-card {
    background: #f8f9fa;
    padding: 20px;
    border-radius: 10px;
    margin: 20px 0;
    border-left: 4px solid #FF6B35;
}

.exercise-header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 15px;
}

.exercise-difficulty {
    background: #FF6B35;
    color: white;
    padding: 5px 10px;
    border-radius: 15px;
    font-size: 12px;
}

.exercise-timer {
    text-align: center;
    margin: 20px 0;
}

.timer-display {
    font-size: 48px;
    font-weight: bold;
    color: #FF6B35;
    margin: 20px 0;
}

.posture-guide {
    background: #e8f5e8;
    padding: 20px;
    border-radius: 10px;
    margin: 20px 0;
}

.posture-steps {
    margin: 15px 0;
}

.posture-step {
    display: flex;
    align-items: center;
    margin: 10px 0;
    padding: 10px;
    background: white;
    border-radius: 8px;
}

.step-number {
    background: #4CAF50;
    color: white;
    width: 25px;
    height: 25px;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-right: 10px;
    font-size: 14px;
    font-weight: bold;
}

.breathing-techniques {
    background: #e3f2fd;
    padding: 20px;
    border-radius: 10px;
    margin: 20px 0;
}

.breathing-exercises {
    margin: 15px 0;
}

.breathing-exercise {
    background: white;
    padding: 15px;
    border-radius: 8px;
    margin: 10px 0;
    cursor: pointer;
    transition: all 0.3s;
}

.breathing-exercise:hover {
    transform: translateY(-2px);
    box-shadow: 0 5px 15px rgba(0,0,0,0.1);
}

.voice-analysis {
    background: #fff3cd;
    padding: 20px;
    border-radius: 10px;
    margin: 20px 0;
    border-left: 4px solid #ffc107;
}

.analysis-results {
    margin: 15px 0;
}

.analysis-item {
    display: flex;
    align-items: center;
    margin: 15px 0;
}

.analysis-label {
    width: 120px;
    font-size: 14px;
    color: #333;
}

.analysis-bar {
    flex: 1;
    background: #e0e0e0;
    height: 8px;
    border-radius: 4px;
    margin: 0 15px;
    overflow: hidden;
}

.analysis-fill {
    background: linear-gradient(90deg, #4CAF50, #8BC34A);
    height: 100%;
    transition: width 0.5s ease;
}

.analysis-value {
    width: 40px;
    text-align: right;
    font-weight: bold;
    color: #333;
}

.voice-progress {
    background: #f8f9fa;
    padding: 20px;
    border-radius: 10px;
    margin: 20px 0;
}

.progress-stats {
    display: flex;
    justify-content: space-between;
    margin-top: 15px;
}

.progress-stat {
    text-align: center;
}

.stat-value {
    font-size: 20px;
    font-weight: bold;
    color: #FF6B35;
}

.stat-label {
    font-size: 12px;
    color: #666;
    margin-top: 5px;
}

.breathing-animation {
    display: flex;
    justify-content: center;
    align-items: center;
    height: 200px;
    margin: 30px 0;
}

.breathing-circle {
    width: 150px;
    height: 150px;
    border-radius: 50%;
    background: linear-gradient(135deg, #667eea, #764ba2);
    display: flex;
    align-items: center;
    justify-content: center;
    animation: breathe 8s infinite ease-in-out;
}

.breathing-text {
    color: white;
    font-size: 18px;
    font-weight: bold;
}

.breathing-timer {
    text-align: center;
    margin: 20px 0;
}

.breathing-time {
    font-size: 36px;
    font-weight: bold;
    color: #667eea;
}

.breathing-phase {
    font-size: 16px;
    color: #666;
    margin-top: 10px;
}

.breathing-instructions {
    text-align: center;
    margin: 20px 0;
    padding: 15px;
    background: #f8f9fa;
    border-radius: 10px;
}

.lesson-content-card {
    background: #f8f9fa;
    padding: 20px;
    border-radius: 10px;
    margin-bottom: 20px;
}

.exercises-section {
    margin: 15px 0;
}

.exercise-item {
    margin: 10px 0;
    padding: 10px;
    background: white;
    border-radius: 5px;
}

.ai-tip {
    background: #e8f5e8;
    padding: 15px;
    border-radius: 10px;
    margin-top: 15px;
}

@keyframes breathe {
    0%, 100% {
        transform: scale(1);
        background: linear-gradient(135deg, #667eea, #764ba2);
    }
    25% {
        transform: scale(1.2);
        background: linear-gradient(135deg, #4CAF50, #8BC34A);
    }
    50% {
        transform: scale(1);
        background: linear-gradient(135deg, #ff9800, #ffc107);
    }
    75% {
        transform: scale(0.8);
        background: linear-gradient(135deg, #f44336, #e91e63);
    }
}

@keyframes pulse {
    0% {
        transform: scale(1);
        opacity: 1;
    }
    50% {
        transform: scale(1.05);
        opacity: 0.8;
    }
    100% {
        transform: scale(1);
        opacity: 1;
    }
}

.pulse {
    animation: pulse 2s infinite;
}

@media (max-width: 480px) {
    body {
        padding: 10px;
    }
    
    .container {
        border-radius: 15px;
    }
    
    .header {
        padding: 20px 15px;
    }
    
    .content {
        padding: 15px;
    }
    
    .skill-grid {
        grid-template-columns: 1fr;
    }
    
    .level-grid {
        grid-template-columns: 1fr;
    }
    
    .analytics-grid {
        flex-direction: column;
        gap: 15px;
    }
    
    .progress-stats {
        flex-direction: column;
        gap: 15px;
    }
    
    .analysis-item {
        flex-direction: column;
        align-items: flex-start;
    }
    
    .analysis-label {
        width: 100%;
        margin-bottom: 5px;
    }
    
    .analysis-bar {
        width: 100%;
        margin: 5px 0;
    }
    
    .timer-display {
        font-size: 36px;
    }
    
    .breathing-circle {
        width: 120px;
        height: 120px;
    }
}
```
