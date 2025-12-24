<!DOCTYPE html>
<html lang="ru">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Connect Ai Bot</title>
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    <style>
        *{box-sizing:border-box;margin:0;padding:0}
        body{font-family:-apple-system,BlinkMacSystemFont,'Segoe UI',Roboto,Helvetica,Arial,sans-serif;background-color:#0a0a0a;color:#e1e1e1;height:100vh;overflow:hidden}
        .app-container{display:flex;flex-direction:column;height:100vh;max-width:100%;margin:0 auto}
        .header{background-color:#1a1a1a;padding:12px 16px;border-bottom:1px solid #2d2d2d;display:flex;align-items:center;justify-content:space-between;box-shadow:0 1px 10px rgba(0,0,0,0.3);z-index:10}
        .logo{display:flex;align-items:center;gap:10px;flex:1;min-width:0}
        .logo-icon{width:32px;height:32px;background:linear-gradient(135deg,#0088cc,#00a8ff);border-radius:50%;display:flex;align-items:center;justify-content:center;flex-shrink:0}
        .logo-icon i{color:white;font-size:16px}
        .logo-text{font-size:16px;font-weight:600;background:linear-gradient(135deg,#0088cc,#00a8ff);-webkit-background-clip:text;background-clip:text;color:transparent;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
        .connection-status{display:flex;align-items:center;gap:6px;padding:6px 10px;background-color:#2d2d2d;border-radius:16px;font-size:12px;flex-shrink:0}
        .status-dot{width:8px;height:8px;border-radius:50%;background-color:#ff3b30}
        .status-dot.connected{background-color:#34c759;box-shadow:0 0 6px #34c759}
        .status-dot.connecting{background-color:#ff9500;animation:pulse 1.5s infinite}
        @keyframes pulse{0%,100%{opacity:1}50%{opacity:0.5}}
        .main-content{display:flex;flex:1;overflow:hidden}
        .sidebar{width:300px;background-color:#1a1a1a;border-right:1px solid #2d2d2d;padding:16px;overflow-y:auto;display:flex;flex-direction:column;gap:16px;transition:all 0.3s ease}
        .connection-form{background-color:#2d2d2d;border-radius:12px;padding:16px;box-shadow:0 4px 12px rgba(0,0,0,0.2)}
        .form-title{font-size:15px;font-weight:600;margin-bottom:14px;color:#e1e1e1;display:flex;align-items:center;gap:8px}
        .form-title i{color:#0088cc}
        .input-group{margin-bottom:14px}
        .input-group label{display:block;font-size:13px;color:#999;margin-bottom:6px}
        .input-group input{width:100%;padding:10px 12px;background-color:#3d3d3d;border:1px solid #4d4d4d;border-radius:8px;color:#e1e1e1;font-size:14px;transition:border 0.2s}
        .input-group input:focus{outline:none;border-color:#0088cc}
        .connect-btn{width:100%;padding:12px;background:linear-gradient(135deg,#0088cc,#0066aa);color:white;border:none;border-radius:8px;font-size:15px;font-weight:600;cursor:pointer;transition:all 0.2s;display:flex;align-items:center;justify-content:center;gap:8px}
        .connect-btn:hover{background:linear-gradient(135deg,#0099dd,#0077bb)}
        .connect-btn:active{transform:translateY(1px)}
        .connect-btn:disabled{background:#3d3d3d;color:#777;cursor:not-allowed;transform:none}
        .ai-settings{background-color:#2d2d2d;border-radius:12px;padding:16px;box-shadow:0 4px 12px rgba(0,0,0,0.2)}
        .ai-settings-title{font-size:15px;font-weight:600;margin-bottom:14px;color:#e1e1e1;display:flex;align-items:center;gap:8px}
        .ai-settings-title i{color:#ff9500}
        .icon-selection{display:grid;grid-template-columns:repeat(4,1fr);gap:8px;margin-bottom:14px}
        .icon-option{width:40px;height:40px;background-color:#3d3d3d;border:2px solid #4d4d4d;border-radius:50%;display:flex;align-items:center;justify-content:center;cursor:pointer;transition:all 0.2s;font-size:18px;color:#e1e1e1}
        .icon-option:hover{background-color:#4d4d4d;transform:scale(1.1)}
        .icon-option.selected{background-color:#0088cc;border-color:#00a8ff;color:white;transform:scale(1.1)}
        .icon-option.custom{position:relative;background:linear-gradient(45deg,#ff6b6b,#ffa8a8)}
        .icon-option.custom i{font-size:16px}
        .icon-input{width:100%;padding:10px 12px;background-color:#3d3d3d;border:1px solid #4d4d4d;border-radius:8px;color:#e1e1e1;font-size:14px;margin-bottom:14px;display:none}
        .icon-input.show{display:block}
        .instructions{background-color:#2d2d2d;border-radius:12px;padding:16px;box-shadow:0 4px 12px rgba(0,0,0,0.2)}
        .instructions h3{font-size:15px;font-weight:600;margin-bottom:12px;color:#e1e1e1}
        .instructions ol{padding-left:16px;font-size:13px;color:#999;line-height:1.5}
        .instructions li{margin-bottom:6px}
        .chat-container{flex:1;display:flex;flex-direction:column;background-color:#0a0a0a;position:relative;overflow:hidden}
        .chat-header{background-color:#1a1a1a;padding:12px 16px;border-bottom:1px solid #2d2d2d;display:flex;align-items:center;gap:10px}
        .chat-avatar{width:42px;height:42px;background:linear-gradient(135deg,#34c759,#2ecc71);border-radius:50%;display:flex;align-items:center;justify-content:center;flex-shrink:0;transition:all 0.3s}
        .chat-avatar i{color:white;font-size:20px}
        .chat-info{flex:1;min-width:0}
        .chat-info h2{font-size:17px;font-weight:600;color:#e1e1e1;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
        .chat-info p{font-size:13px;color:#999;margin-top:2px;white-space:nowrap;overflow:hidden;text-overflow:ellipsis}
        .clear-history-btn{background-color:#3d3d3d;color:#e1e1e1;border:1px solid #4d4d4d;border-radius:8px;padding:8px 12px;font-size:13px;cursor:pointer;transition:all 0.2s;display:flex;align-items:center;gap:6px;margin-left:auto;flex-shrink:0}
        .clear-history-btn:hover{background-color:#4d4d4d;border-color:#ff3b30;color:#ff3b30}
        .chat-messages{flex:1;overflow-y:auto;padding:16px;display:flex;flex-direction:column;gap:12px;background-color:#0a0a0a}
        .message{max-width:85%;padding:10px 14px;border-radius:16px;line-height:1.4;word-wrap:break-word;position:relative;animation:fadeIn 0.3s ease}
        @keyframes fadeIn{from{opacity:0;transform:translateY(10px)}to{opacity:1;transform:translateY(0)}}
        .user-message{align-self:flex-end;background-color:#0088cc;color:white;border-bottom-right-radius:4px;box-shadow:0 2px 8px rgba(0,136,204,0.3)}
        .ai-message{align-self:flex-start;background-color:#2d2d2d;color:#e1e1e1;border-bottom-left-radius:4px;box-shadow:0 2px 8px rgba(0,0,0,0.2)}
        .message-time{font-size:10px;color:rgba(255,255,255,0.6);margin-top:4px;text-align:right}
        .ai-message .message-time{color:#999}
        .typing-indicator{align-self:flex-start;background-color:#2d2d2d;border-radius:16px;border-bottom-left-radius:4px;padding:10px 14px;display:none;margin-bottom:10px;box-shadow:0 2px 8px rgba(0,0,0,0.2)}
        .typing-indicator.active{display:flex}
        .typing-dots{display:flex;gap:3px;align-items:center}
        .typing-dots span{width:6px;height:6px;border-radius:50%;background-color:#999;animation:typing 1.4s infinite ease-in-out both}
        .typing-dots span:nth-child(1){animation-delay:-0.32s}
        .typing-dots span:nth-child(2){animation-delay:-0.16s}
        @keyframes typing{0%,80%,100%{transform:scale(0.6);opacity:0.5}40%{transform:scale(1);opacity:1}}
        .chat-input-area{padding:12px 16px;background-color:#1a1a1a;border-top:1px solid #2d2d2d;display:flex;gap:10px;align-items:flex-end}
        .chat-input-wrapper{flex:1;background-color:#2d2d2d;border-radius:20px;padding:6px 14px;display:flex;align-items:center;border:1px solid transparent}
        .chat-input-wrapper:focus-within{border-color:#0088cc}
        .chat-input{flex:1;background:transparent;border:none;color:#e1e1e1;font-size:14px;resize:none;max-height:100px;min-height:20px;line-height:1.4;padding:6px 0}
        .chat-input:focus{outline:none}
        .chat-actions{display:flex;gap:6px;align-items:center}
        .send-button{width:40px;height:40px;background:linear-gradient(135deg,#0088cc,#0066aa);border:none;border-radius:50%;color:white;font-size:16px;cursor:pointer;display:flex;align-items:center;justify-content:center;transition:all 0.2s;flex-shrink:0}
        .send-button:hover{background:linear-gradient(135deg,#0099dd,#0077bb)}
        .send-button:active{transform:scale(0.95)}
        .send-button:disabled{background:#3d3d3d;color:#777;cursor:not-allowed;transform:none}
        .mobile-menu-btn{display:none;background:none;border:none;color:#e1e1e1;font-size:18px;cursor:pointer;padding:6px;margin-right:8px}
        .sidebar-overlay{display:none;position:fixed;top:0;left:0;right:0;bottom:0;background-color:rgba(0,0,0,0.7);z-index:100}
        .sidebar-overlay.active{display:block}
        .error-message{background-color:rgba(255,59,48,0.1);border:1px solid rgba(255,59,48,0.3);border-radius:8px;padding:12px;margin-top:12px;font-size:12px;color:#ff7b72;display:none}
        .error-message.show{display:block;animation:shake 0.5s ease}
        @keyframes shake{0%,100%{transform:translateX(0)}25%{transform:translateX(-5px)}75%{transform:translateX(5px)}}
        .error-message i{margin-right:6px}
        .retry-btn{background:rgba(255,59,48,0.2);border:1px solid rgba(255,59,48,0.5);color:#ff7b72;padding:6px 12px;border-radius:6px;font-size:11px;cursor:pointer;margin-top:8px;display:inline-flex;align-items:center;gap:4px;transition:all 0.2s}
        .retry-btn:hover{background:rgba(255,59,48,0.3)}
        .connection-info-box{margin-top:12px;padding:10px;background:rgba(0,0,0,0.3);border-radius:8px;border-left:3px solid #34c759;display:none}
        .connection-info-box.show{display:block}
        .connection-info-title{font-size:11px;color:#999;margin-bottom:4px}
        .connection-info-details{font-size:12px;color:#e1e1e1;display:flex;flex-direction:column;gap:3px}
        .connection-success{color:#34c759}
        .connection-error{color:#ff3b30}
        .custom-icon-input{display:none;margin-top:10px}
        .custom-icon-input.show{display:block}
        .custom-icon-input input{width:100%;padding:8px 12px;background-color:#3d3d3d;border:1px solid #4d4d4d;border-radius:6px;color:#e1e1e1;font-size:13px}
        .welcome-message{text-align:center;padding:30px 16px;color:#999;font-size:14px}
        .welcome-message i{font-size:36px;margin-bottom:12px;color:#0088cc;opacity:0.7}
        .sidebar-header{display:none;align-items:center;justify-content:space-between;padding-bottom:12px;border-bottom:1px solid #2d2d2d;margin-bottom:16px}
        .sidebar-close-btn{background:none;border:none;color:#e1e1e1;font-size:20px;cursor:pointer;padding:4px}
        ::-webkit-scrollbar{width:6px}
        ::-webkit-scrollbar-track{background:#1a1a1a}
        ::-webkit-scrollbar-thumb{background:#3d3d3d;border-radius:3px}
        ::-webkit-scrollbar-thumb:hover{background:#4d4d4d}
        
        @media (max-width:768px){
            .sidebar{position:fixed;top:0;left:-100%;width:100%;height:100%;z-index:101;transition:left 0.3s ease;padding:16px}
            .sidebar.active{left:0}
            .sidebar-header{display:flex}
            .mobile-menu-btn{display:block}
            .logo-text{font-size:15px}
            .message{max-width:90%;padding:8px 12px;font-size:14px}
            .chat-input-area{padding:10px 14px}
            .connection-status{font-size:11px;padding:5px 8px}
            .clear-history-btn{padding:6px 10px;font-size:12px}
            .icon-selection{grid-template-columns:repeat(5,1fr)}
        }
        @media (max-width:480px){
            .header{padding:10px 14px}
            .chat-header{padding:10px 14px}
            .chat-messages{padding:14px;gap:10px}
            .message{max-width:92%;padding:8px 10px;font-size:13px}
            .message-time{font-size:9px}
            .connection-form,.instructions,.ai-settings{padding:14px}
            .chat-actions{gap:5px}
            .send-button{width:38px;height:38px;font-size:15px}
            .logo-icon{width:30px;height:30px}
            .logo-text{font-size:14px}
            .clear-history-btn{padding:5px 8px;font-size:11px}
            .icon-selection{grid-template-columns:repeat(4,1fr);gap:6px}
            .icon-option{width:36px;height:36px;font-size:16px}
        }
        @media (max-width:360px){
            .logo-text{font-size:13px}
            .connection-status{font-size:10px}
            .mobile-menu-btn{font-size:16px;padding:4px;margin-right:4px}
            .clear-history-btn{padding:4px 6px;font-size:10px}
            .icon-selection{grid-template-columns:repeat(3,1fr)}
        }
    </style>
</head>
<body>
    <div class="app-container">
        <header class="header">
            <button class="mobile-menu-btn" id="mobile-menu-btn">
                <i class="fas fa-bars"></i>
            </button>
            
            <div class="logo">
                <div class="logo-icon">
                    <i class="fas fa-robot"></i>
                </div>
                <div class="logo-text">Connect Ai Bot</div>
            </div>
            
            <div class="connection-status">
                <div class="status-dot" id="status-dot"></div>
                <span id="status-text">Не подключено</span>
            </div>
        </header>
        
        <div class="main-content">
            <div class="sidebar" id="sidebar">
                <div class="sidebar-header">
                    <h3>Настройки подключения</h3>
                    <button class="sidebar-close-btn" id="sidebar-close-btn">
                        <i class="fas fa-times"></i>
                    </button>
                </div>
                
                <div class="connection-form">
                    <h3 class="form-title">
                        <i class="fas fa-plug"></i>
                        Подключение к серверу
                    </h3>
                    
                    <div class="input-group">
                        <label for="ip-address">IP-адрес сервера</label>
                        <input type="text" id="ip-address" placeholder="Например: 127.0.0.1 или 26.24.239.213">
                    </div>
                    
                    <div class="input-group">
                        <label for="port">Порт сервера</label>
                        <input type="number" id="port" placeholder="1234" min="1" max="65535">
                    </div>
                    
                    <button class="connect-btn" id="connect-btn">
                        <i class="fas fa-plug"></i>
                        <span>Подключиться</span>
                    </button>
                    
                    <div class="error-message" id="error-message">
                        <div>
                            <i class="fas fa-exclamation-triangle"></i>
                            <span id="error-text">Не удалось подключиться к серверу</span>
                        </div>
                        <button class="retry-btn" id="retry-btn">
                            <i class="fas fa-redo"></i>
                            Попробовать снова
                        </button>
                    </div>
                    
                    <div class="connection-info-box" id="connection-info-box">
                        <div class="connection-info-title">Подключено к:</div>
                        <div class="connection-info-details">
                            <div>Сервер: <span id="server-info">127.0.0.1:1234</span></div>
                            <div>Статус: <span class="connection-success" id="connection-details">Активно</span></div>
                        </div>
                    </div>
                </div>
                
                <div class="ai-settings">
                    <h3 class="ai-settings-title">
                        <i class="fas fa-cog"></i>
                        Настройки AI
                    </h3>
                    
                    <div class="input-group">
                        <label for="ai-name">Имя AI</label>
                        <input type="text" id="ai-name" placeholder="Например: LM Studio AI или Друг">
                    </div>
                    
                    <div class="input-group">
                        <label for="ai-role">Роль AI</label>
                        <input type="text" id="ai-role" placeholder="Например: Помощник, Друг, Эксперт">
                    </div>
                    
                    <div class="input-group">
                        <label>Иконка AI</label>
                        <div class="icon-selection" id="icon-selection">
                            <div class="icon-option selected" data-icon="fas fa-brain">
                                <i class="fas fa-brain"></i>
                            </div>
                            <div class="icon-option" data-icon="fas fa-robot">
                                <i class="fas fa-robot"></i>
                            </div>
                            <div class="icon-option" data-icon="fas fa-user-circle">
                                <i class="fas fa-user-circle"></i>
                            </div>
                            <div class="icon-option" data-icon="fas fa-user-tie">
                                <i class="fas fa-user-tie"></i>
                            </div>
                            <div class="icon-option" data-icon="fas fa-graduation-cap">
                                <i class="fas fa-graduation-cap"></i>
                            </div>
                            <div class="icon-option" data-icon="fas fa-code">
                                <i class="fas fa-code"></i>
                            </div>
                            <div class="icon-option" data-icon="fas fa-gamepad">
                                <i class="fas fa-gamepad"></i>
                            </div>
                            <div class="icon-option custom" data-icon="custom">
                                <i class="fas fa-plus"></i>
                            </div>
                        </div>
                        <div class="custom-icon-input" id="custom-icon-input">
                            <input type="text" id="custom-icon-text" placeholder="Код иконки FontAwesome (например: fas fa-star)">
                        </div>
                    </div>
                    
                    <button class="connect-btn" id="save-ai-settings">
                        <i class="fas fa-save"></i>
                        <span>Сохранить настройки AI</span>
                    </button>
                </div>
                
                <div class="instructions">
                    <h3>Как подключиться:</h3>
                    <ol>
                        <li>Запустите LM Studio</li>
                        <li>Загрузите модель</li>
                        <li>Перейдите в "Local Server"</li>
                        <li>Нажмите "Start Server"</li>
                        <li>Введите IP и порт</li>
                        <li>Настройте AI как хотите</li>
                        <li>Нажмите "Подключиться"</li>
                    </ol>
                    <p style="margin-top:10px;font-size:12px;color:#666">
                        <i class="fas fa-info-circle"></i> Назовите AI как хотите: "Друг", "Помощник" и т.д.
                    </p>
                </div>
            </div>
            
            <div class="sidebar-overlay" id="sidebar-overlay"></div>
            
            <div class="chat-container">
                <div class="chat-header">
                    <div class="chat-avatar" id="chat-avatar">
                        <i class="fas fa-brain"></i>
                    </div>
                    <div class="chat-info">
                        <h2 id="ai-name-display">LM Studio AI</h2>
                        <p id="connection-info">Ожидание подключения...</p>
                    </div>
                    <button class="clear-history-btn" id="clear-history-btn" title="Очистить историю">
                        <i class="fas fa-trash"></i>
                        Очистить
                    </button>
                </div>
                
                <div class="chat-messages" id="chat-messages">
                    <div class="welcome-message" id="welcome-message">
                        <i class="fas fa-robot"></i>
                        <p>Подключитесь к серверу LM Studio, чтобы начать общение</p>
                    </div>
                </div>
                
                <div class="typing-indicator" id="typing-indicator">
                    <div class="typing-dots">
                        <span></span>
                        <span></span>
                        <span></span>
                    </div>
                </div>
                
                <div class="chat-input-area">
                    <div class="chat-input-wrapper">
                        <textarea class="chat-input" id="chat-input" placeholder="Напишите сообщение..." rows="1" disabled></textarea>
                    </div>
                    <div class="chat-actions">
                        <button class="send-button" id="send-btn" disabled>
                            <i class="fas fa-paper-plane"></i>
                        </button>
                    </div>
                </div>
            </div>
        </div>
    </div>

    <script>
        document.addEventListener('DOMContentLoaded',function(){
            const ipAddressInput=document.getElementById('ip-address')
            const portInput=document.getElementById('port')
            const connectBtn=document.getElementById('connect-btn')
            const statusDot=document.getElementById('status-dot')
            const statusText=document.getElementById('status-text')
            const chatMessages=document.getElementById('chat-messages')
            const chatInput=document.getElementById('chat-input')
            const sendBtn=document.getElementById('send-btn')
            const typingIndicator=document.getElementById('typing-indicator')
            const connectionInfo=document.getElementById('connection-info')
            const welcomeMessage=document.getElementById('welcome-message')
            const mobileMenuBtn=document.getElementById('mobile-menu-btn')
            const sidebar=document.getElementById('sidebar')
            const sidebarOverlay=document.getElementById('sidebar-overlay')
            const clearHistoryBtn=document.getElementById('clear-history-btn')
            const errorMessage=document.getElementById('error-message')
            const errorText=document.getElementById('error-text')
            const retryBtn=document.getElementById('retry-btn')
            const connectionInfoBox=document.getElementById('connection-info-box')
            const serverInfo=document.getElementById('server-info')
            const connectionDetails=document.getElementById('connection-details')
            const aiNameInput=document.getElementById('ai-name')
            const aiRoleInput=document.getElementById('ai-role')
            const aiNameDisplay=document.getElementById('ai-name-display')
            const chatAvatar=document.getElementById('chat-avatar')
            const iconSelection=document.getElementById('icon-selection')
            const customIconInput=document.getElementById('custom-icon-input')
            const customIconText=document.getElementById('custom-icon-text')
            const saveAiSettingsBtn=document.getElementById('save-ai-settings')
            const iconOptions=document.querySelectorAll('.icon-option')
            const sidebarCloseBtn=document.getElementById('sidebar-close-btn')
            
            let isConnected=false
            let connectionUrl=''
            let conversationHistory=[]
            let currentSettings={ip:'127.0.0.1',port:'1234'}
            let aiSettings={name:'LM Studio AI',role:'Помощник',icon:'fas fa-brain',iconClass:'fas fa-brain'}
            let reconnectAttempts=0
            const MAX_RECONNECT_ATTEMPTS=3
            
            function isValidIP(ip){
                const ipv4Regex=/^(\d{1,3}\.){3}\d{1,3}$/
                if(!ipv4Regex.test(ip))return false
                const parts=ip.split('.')
                for(let part of parts){
                    const num=parseInt(part,10)
                    if(num<0||num>255)return false
                    if(part.length>1&&part[0]==='0')return false
                }
                return true
            }
            
            function loadSettings(){
                const savedIp=localStorage.getItem('lmStudioIp')
                const savedPort=localStorage.getItem('lmStudioPort')
                if(savedIp&&isValidIP(savedIp))currentSettings.ip=savedIp
                if(savedPort)currentSettings.port=savedPort
                ipAddressInput.value=currentSettings.ip
                portInput.value=currentSettings.port
                const savedAiName=localStorage.getItem('aiName')
                const savedAiRole=localStorage.getItem('aiRole')
                const savedAiIcon=localStorage.getItem('aiIcon')
                const savedAiIconClass=localStorage.getItem('aiIconClass')
                if(savedAiName)aiSettings.name=savedAiName
                if(savedAiRole)aiSettings.role=savedAiRole
                if(savedAiIcon)aiSettings.icon=savedAiIcon
                if(savedAiIconClass)aiSettings.iconClass=savedAiIconClass
                aiNameInput.value=aiSettings.name
                aiRoleInput.value=aiSettings.role
                applyAiSettings()
            }
            
            function saveConnectionSettings(){
                const ip=ipAddressInput.value.trim()
                const port=portInput.value.trim()
                if(ip&&port&&isValidIP(ip)){
                    localStorage.setItem('lmStudioIp',ip)
                    localStorage.setItem('lmStudioPort',port)
                    currentSettings={ip,port}
                }
            }
            
            function saveAiSettings(){
                const name=aiNameInput.value.trim()||'LM Studio AI'
                const role=aiRoleInput.value.trim()||'Помощник'
                aiSettings.name=name
                aiSettings.role=role
                localStorage.setItem('aiName',name)
                localStorage.setItem('aiRole',role)
                localStorage.setItem('aiIcon',aiSettings.icon)
                localStorage.setItem('aiIconClass',aiSettings.iconClass)
                applyAiSettings()
                showNotification('Настройки AI сохранены!')
            }
            
            function applyAiSettings(){
                aiNameDisplay.textContent=aiSettings.name
                connectionInfo.textContent=isConnected?`Подключено как ${aiSettings.role}`:'Ожидание подключения...'
                const avatarIcon=chatAvatar.querySelector('i')
                avatarIcon.className=aiSettings.iconClass
                setAvatarGradient(aiSettings.icon)
            }
            
            function setAvatarGradient(iconType){
                const gradients={
                    'fas fa-brain':'linear-gradient(135deg,#34c759,#2ecc71)',
                    'fas fa-robot':'linear-gradient(135deg,#007aff,#5856d6)',
                    'fas fa-user-circle':'linear-gradient(135deg,#ff2d55,#ff375f)',
                    'fas fa-user-tie':'linear-gradient(135deg,#5ac8fa,#007aff)',
                    'fas fa-graduation-cap':'linear-gradient(135deg,#ff9500,#ffcc00)',
                    'fas fa-code':'linear-gradient(135deg,#5856d6,#af52de)',
                    'fas fa-gamepad':'linear-gradient(135deg,#ff3b30,#ff9500)',
                    'default':'linear-gradient(135deg,#34c759,#2ecc71)'
                }
                const gradient=gradients[iconType]||gradients['default']
                chatAvatar.style.background=gradient
            }
            
            function showNotification(message){
                const notification=document.createElement('div')
                notification.style.cssText='position:fixed;top:20px;right:20px;background:#34c759;color:white;padding:12px 20px;border-radius:8px;z-index:1000;box-shadow:0 4px 12px rgba(0,0,0,0.3);animation:slideIn 0.3s ease'
                notification.innerHTML=`<div style="display:flex;align-items:center;gap:8px"><i class="fas fa-check-circle"></i><span>${message}</span></div>`
                document.body.appendChild(notification)
                setTimeout(()=>{
                    notification.style.animation='slideOut 0.3s ease'
                    setTimeout(()=>{if(notification.parentNode)notification.parentNode.removeChild(notification)},300)
                },3000)
                if(!document.querySelector('#notification-styles')){
                    const style=document.createElement('style')
                    style.id='notification-styles'
                    style.textContent='@keyframes slideIn{from{transform:translateX(100%);opacity:0}to{transform:translateX(0);opacity:1}}@keyframes slideOut{from{transform:translateX(0);opacity:1}to{transform:translateX(100%);opacity:0}}'
                    document.head.appendChild(style)
                }
            }
            
            function showError(message){
                errorText.textContent=message
                errorMessage.classList.add('show')
                connectionInfoBox.classList.remove('show')
                statusDot.classList.remove('connected','connecting')
                statusText.textContent='Ошибка'
                connectionInfo.textContent=message
                connectionInfo.classList.remove('connection-success')
                connectionInfo.classList.add('connection-error')
            }
            
            function hideError(){
                errorMessage.classList.remove('show')
            }
            
            function showConnectionInfo(){
                serverInfo.textContent=`${currentSettings.ip}:${currentSettings.port}`
                connectionInfoBox.classList.add('show')
                hideError()
            }
            
            function updateConnectionStatus(connected,connecting=false){
                isConnected=connected
                if(connecting){
                    statusDot.className='status-dot connecting'
                    statusText.textContent='Подключение...'
                    connectBtn.disabled=true
                    chatInput.disabled=true
                    sendBtn.disabled=true
                    chatInput.placeholder='Подключаемся...'
                    connectionInfo.textContent='Подключаемся к серверу...'
                    connectionInfo.classList.remove('connection-success','connection-error')
                    return
                }
                if(connected){
                    statusDot.className='status-dot connected'
                    statusText.textContent='Подключено'
                    connectBtn.innerHTML='<i class="fas fa-unplug"></i><span>Отключиться</span>'
                    chatInput.disabled=false
                    sendBtn.disabled=false
                    chatInput.placeholder='Напишите сообщение...'
                    connectionInfo.textContent=`Подключено как ${aiSettings.role}`
                    connectionInfo.classList.add('connection-success')
                    connectionInfo.classList.remove('connection-error')
                    connectionDetails.textContent='Активно'
                    connectionDetails.className='connection-success'
                    if(welcomeMessage)welcomeMessage.style.display='none'
                    addMessage('ai-message',`✅ Подключение успешно установлено! Я ваш ${aiSettings.role.toLowerCase()} ${aiSettings.name}. Готов помочь!`,false)
                    saveConnectionSettings()
                    showConnectionInfo()
                    reconnectAttempts=0
                }else{
                    statusDot.className='status-dot'
                    statusText.textContent='Не подключено'
                    connectBtn.innerHTML='<i class="fas fa-plug"></i><span>Подключиться</span>'
                    chatInput.disabled=true
                    sendBtn.disabled=true
                    chatInput.placeholder='Сначала подключитесь...'
                    connectionInfo.textContent=`Ожидание подключения (${aiSettings.role})`
                    connectionInfo.classList.remove('connection-success','connection-error')
                    connectionInfoBox.classList.remove('show')
                    connectBtn.disabled=false
                    if(welcomeMessage&&chatMessages.children.length<=2)welcomeMessage.style.display='block'
                }
            }
            
            function addMessage(type,text,saveToHistory=true){
                if(welcomeMessage&&welcomeMessage.style.display!=='none')welcomeMessage.style.display='none'
                const messageDiv=document.createElement('div')
                messageDiv.classList.add('message',type)
                const messageText=document.createElement('div')
                messageText.textContent=text
                messageDiv.appendChild(messageText)
                const timeDiv=document.createElement('div')
                timeDiv.classList.add('message-time')
                const now=new Date()
                const timeString=now.getHours().toString().padStart(2,'0')+':'+now.getMinutes().toString().padStart(2,'0')
                timeDiv.textContent=timeString
                messageDiv.appendChild(timeDiv)
                chatMessages.appendChild(messageDiv)
                chatMessages.scrollTop=chatMessages.scrollHeight
                if(saveToHistory){
                    if(type==='user-message')conversationHistory.push({role:'user',content:text})
                    else if(type==='ai-message')conversationHistory.push({role:'assistant',content:text})
                    if(conversationHistory.length>20)conversationHistory=conversationHistory.slice(-20)
                }
            }
            
            function buildSimpleMessage(userMessage){
                return{model:'local-model',messages:[{role:'user',content:userMessage}],temperature:0.7,max_tokens:500,stream:false}
            }
            
            async function sendMessage(){
                const message=chatInput.value.trim()
                if(!message||!isConnected)return
                addMessage('user-message',message)
                chatInput.value=''
                chatInput.style.height='auto'
                typingIndicator.classList.add('active')
                try{
                    const payload=buildSimpleMessage(message)
                    const response=await fetch(`${connectionUrl}/v1/chat/completions`,{method:'POST',headers:{'Content-Type':'application/json'},body:JSON.stringify(payload)})
                    if(!response.ok){
                        const errorText=await response.text()
                        throw new Error(`Ошибка ${response.status}: ${errorText.substring(0,100)}`)
                    }
                    const data=await response.json()
                    const aiResponse=data.choices[0].message.content
                    addMessage('ai-message',aiResponse)
                }catch(error){
                    console.error('Ошибка при отправке:',error)
                    if(error.message.includes('400')){
                        addMessage('ai-message','⚠️ Ошибка формата запроса. Попробуйте отправить сообщение снова.')
                        connectionDetails.textContent='Ошибка запроса'
                        connectionDetails.className='connection-error'
                    }else if(error.message.includes('NetworkError')||error.message.includes('Failed to fetch')){
                        addMessage('ai-message','🔌 Потеряно соединение с сервером. Проверьте LM Studio.')
                        updateConnectionStatus(false)
                        showError('Потеряно соединение с сервером')
                    }else{
                        addMessage('ai-message',`❌ Ошибка: ${error.message}`)
                    }
                }finally{
                    typingIndicator.classList.remove('active')
                }
            }
            
            async function testConnection(url){
                try{
                    const controller=new AbortController()
                    const timeoutId=setTimeout(()=>controller.abort(),8000)
                    const response=await fetch(`${url}/v1/models`,{method:'GET',headers:{'Content-Type':'application/json'},signal:controller.signal})
                    clearTimeout(timeoutId)
                    if(!response.ok)throw new Error(`Сервер недоступен (${response.status})`)
                    return{success:true}
                }catch(error){
                    console.error('Ошибка теста подключения:',error)
                    if(error.name==='AbortError')return{success:false,error:'Таймаут подключения (8 секунд)'}
                    else if(error.message.includes('CORS'))return{success:false,error:'Ошибка CORS. Сервер не разрешает запросы'}
                    else if(error.message.includes('NetworkError'))return{success:false,error:'Сервер не найден или не запущен'}
                    return{success:false,error:error.message||'Не удалось подключиться к серверу'}
                }
            }
            
            async function connectToServer(){
                if(isConnected){
                    updateConnectionStatus(false)
                    addMessage('ai-message','🔌 Подключение разорвано.',false)
                    connectionUrl=''
                    return
                }
                const ip=ipAddressInput.value.trim()
                const port=portInput.value.trim()
                if(!ip||!port){
                    showError('Введите IP-адрес и порт сервера')
                    return
                }
                if(!isValidIP(ip)){
                    showError('Некорректный IP-адрес. Пример: 127.0.0.1 или 26.24.239.213')
                    return
                }
                if(reconnectAttempts>=MAX_RECONNECT_ATTEMPTS){
                    showError('Слишком много неудачных попыток подключения')
                    return
                }
                connectionUrl=`http://${ip}:${port}`
                currentSettings={ip,port}
                updateConnectionStatus(false,true)
                hideError()
                reconnectAttempts++
                try{
                    const result=await testConnection(connectionUrl)
                    if(!result.success)throw new Error(result.error||'Не удалось подключиться к серверу')
                    updateConnectionStatus(true)
                    addMessage('ai-message','🔍 Проверяю доступные модели...',false)
                    const controller=new AbortController()
                    const timeoutId=setTimeout(()=>controller.abort(),5000)
                    const modelsResponse=await fetch(`${connectionUrl}/v1/models`,{signal:controller.signal})
                    clearTimeout(timeoutId)
                    const modelsData=await modelsResponse.json()
                    if(modelsData.data&&modelsData.data.length>0){
                        const modelName=modelsData.data[0].id
                        connectionDetails.textContent=`Модель: ${modelName}`
                        addMessage('ai-message',`✅ Готово! Используется модель: ${modelName}`,false)
                    }else{
                        connectionDetails.textContent='Модель загружена'
                        addMessage('ai-message','✅ Сервер готов к работе!',false)
                    }
                }catch(error){
                    console.error('Ошибка подключения:',error)
                    let errorMsg='Не удалось подключиться к серверу'
                    if(error.message.includes('timeout')||error.message.includes('AbortError'))errorMsg='Сервер не отвечает (таймаут 8 секунд). Проверьте:\n1. Запущен ли LM Studio\n2. Активен ли сервер API\n3. Правильность IP и порта'
                    else if(error.message.includes('CORS'))errorMsg='Ошибка CORS. Убедитесь, что сервер разрешает запросы с этого сайта'
                    else if(error.message.includes('NetworkError'))errorMsg='Сервер не найден. Проверьте:\n1. Правильность IP адреса\n2. Запущен ли сервер LM Studio\n3. Не блокирует ли брандмауэр подключение'
                    showError(errorMsg)
                    updateConnectionStatus(false)
                    if(reconnectAttempts<MAX_RECONNECT_ATTEMPTS)addMessage('ai-message',`⚠️ Попытка подключения ${reconnectAttempts}/${MAX_RECONNECT_ATTEMPTS} не удалась. Проверьте настройки сервера.`,false)
                }
            }
            
            function clearConversationHistory(){
                conversationHistory=[]
                const messages=chatMessages.querySelectorAll('.message')
                messages.forEach(msg=>{
                    if(!msg.classList.contains('ai-message')||!msg.textContent.includes('Подключение установлено')&&!msg.textContent.includes('Ожидание подключения')&&!msg.textContent.includes('Проверяю доступные модели')&&!msg.textContent.includes('Готово!'))msg.remove()
                })
                if(welcomeMessage&&!isConnected)welcomeMessage.style.display='block'
                addMessage('ai-message','🗑️ История чата очищена.',false)
            }
            
            function selectIcon(iconOption){
                iconOptions.forEach(opt=>opt.classList.remove('selected'))
                iconOption.classList.add('selected')
                if(iconOption.dataset.icon==='custom'){
                    customIconInput.classList.add('show')
                    customIconText.focus()
                }else{
                    customIconInput.classList.remove('show')
                    aiSettings.icon=iconOption.dataset.icon
                    aiSettings.iconClass=iconOption.dataset.icon
                    setAvatarGradient(aiSettings.icon)
                }
            }
            
            function handleCustomIcon(){
                const iconCode=customIconText.value.trim()
                if(iconCode){
                    const testIcon=document.createElement('i')
                    testIcon.className=iconCode
                    if(iconCode.startsWith('fas ')||iconCode.startsWith('fab ')||iconCode.startsWith('far ')){
                        aiSettings.icon='custom'
                        aiSettings.iconClass=iconCode
                        const customOption=document.querySelector('.icon-option.custom')
                        const customIcon=customOption.querySelector('i')
                        customIcon.className=iconCode
                        setAvatarGradient('custom')
                    }else{
                        showNotification('Используйте код FontAwesome (например: fas fa-star)')
                    }
                }
            }
            
            function openSidebar(){
                sidebar.classList.add('active')
                sidebarOverlay.classList.add('active')
                document.body.style.overflow='hidden'
            }
            
            function closeSidebar(){
                sidebar.classList.remove('active')
                sidebarOverlay.classList.remove('active')
                document.body.style.overflow='auto'
            }
            
            loadSettings()
            
            connectBtn.addEventListener('click',connectToServer)
            retryBtn.addEventListener('click',connectToServer)
            sendBtn.addEventListener('click',sendMessage)
            clearHistoryBtn.addEventListener('click',clearConversationHistory)
            saveAiSettingsBtn.addEventListener('click',saveAiSettings)
            
            iconOptions.forEach(option=>{
                option.addEventListener('click',()=>selectIcon(option))
            })
            
            customIconText.addEventListener('change',handleCustomIcon)
            customIconText.addEventListener('blur',handleCustomIcon)
            
            chatInput.addEventListener('keydown',function(e){
                if(e.key==='Enter'&&!e.shiftKey){
                    e.preventDefault()
                    sendMessage()
                }
            })
            
            chatInput.addEventListener('input',function(){
                this.style.height='auto'
                this.style.height=(this.scrollHeight)+'px'
                if(this.value.trim())sendBtn.disabled=false
                else sendBtn.disabled=!isConnected
            })
            
            ipAddressInput.addEventListener('input',saveConnectionSettings)
            portInput.addEventListener('input',saveConnectionSettings)
            aiNameInput.addEventListener('input',()=>{
                aiNameDisplay.textContent=aiNameInput.value||'LM Studio AI'
            })
            
            mobileMenuBtn.addEventListener('click',openSidebar)
            sidebarCloseBtn.addEventListener('click',closeSidebar)
            sidebarOverlay.addEventListener('click',closeSidebar)
            
            window.addEventListener('resize',function(){
                if(window.innerWidth>768)closeSidebar()
            })
            
            setTimeout(()=>{
                if(!isConnected)addMessage('ai-message',`👋 Привет! Я ваш будущий ${aiSettings.role.toLowerCase()} ${aiSettings.name}. Подключитесь к серверу LM Studio через боковую панель.`,false)
            },1000)
        })
    </script>
</body>
</html>
