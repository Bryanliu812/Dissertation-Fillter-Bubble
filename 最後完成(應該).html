<!DOCTYPE html>
<html lang="zh-TW">
<head>
  <meta charset="UTF-8">
  <title>社群媒體推送模擬器</title>
  <style>
    body {
      font-family: 'Segoe UI', 'Microsoft JhengHei', sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f0f2f5;
      color: #1c1e21;
    }
    
    .container {
      max-width: 500px;
      margin: 20px auto;
      background: white;
      border-radius: 8px;
      box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
      overflow: hidden;
    }
    
    .header {
      background: #4267B2;
      color: white;
      padding: 15px;
      text-align: center;
      position: relative;
    }
    
    .feed {
      padding: 10px;
      height: 400px;
      overflow-y: auto;
    }
    
    .post {
      margin-bottom: 15px;
      border-bottom: 1px solid #ddd;
      padding-bottom: 15px;
      position: relative;
    }
    
    .profile {
      display: flex;
      align-items: center;
      margin-bottom: 10px;
    }
    
    .profile-img {
      width: 40px;
      height: 40px;
      border-radius: 50%;
      background-color: #ddd;
      margin-right: 10px;
      display: flex;
      align-items: center;
      justify-content: center;
      color: #666;
      font-weight: bold;
    }
    
    .name {
      font-weight: bold;
    }
    
    .time {
      color: #65676B;
      font-size: 12px;
    }
    
    .content {
      margin-bottom: 10px;
      line-height: 1.4;
    }
    
    .image {
      width: 100%;
      height: auto;
      max-height: 300px;
      object-fit: cover;
      margin-bottom: 10px;
    }
    
    .actions {
      display: flex;
      justify-content: space-between;
      color: #65676B;
      font-size: 14px;
    }
    
    .action {
      cursor: pointer;
      padding: 5px;
      display: flex;
      align-items: center;
    }
    
    .action:hover {
      background-color: #f2f2f2;
      border-radius: 4px;
    }
    
    .stats {
      display: flex;
      justify-content: space-between;
      color: #65676B;
      font-size: 12px;
      margin-bottom: 8px;
    }
    
    .engagement {
      position: absolute;
      top: 10px;
      right: 10px;
      background: #f0f2f5;
      border-radius: 10px;
      padding: 3px 8px;
      font-size: 11px;
      color: #65676B;
    }
    
    .notification {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: white;
      padding: 15px;
      border-radius: 8px;
      box-shadow: 0 2px 15px rgba(0, 0, 0, 0.2);
      display: none;
      max-width: 300px;
      z-index: 1000;
      animation: slideIn 0.3s forwards;
    }
    
    @keyframes slideIn {
      from {
        transform: translateX(100%);
        opacity: 0;
      }
      to {
        transform: translateX(0);
        opacity: 1;
      }
    }
    
    .controls {
      display: flex;
      justify-content: space-between;
      padding: 10px;
      background: #f5f5f5;
      border-top: 1px solid #ddd;
    }
    
    .stats-container {
      padding: 15px;
      border-top: 1px solid #ddd;
    }
    
    .stats-title {
      font-weight: bold;
      margin-bottom: 10px;
    }
    
    .stat-item {
      display: flex;
      justify-content: space-between;
      margin-bottom: 5px;
    }
    
    .progress-container {
      margin-top: 5px;
      background: #e0e0e0;
      height: 6px;
      border-radius: 3px;
      overflow: hidden;
    }
    
    .progress-bar {
      height: 100%;
      background: #4267B2;
      width: 0%;
      transition: width 0.5s ease;
    }
    
    button {
      padding: 8px 12px;
      border: none;
      border-radius: 4px;
      background: #4267B2;
      color: white;
      cursor: pointer;
      font-size: 14px;
    }
    
    button:hover {
      background: #365899;
    }
    
    .addiction-meter {
      margin-top: 10px;
      text-align: center;
    }
  </style>
</head>
<body>
  <div class="container">
    <div class="header">
      <h2>社群媒體推送模擬器</h2>
      <p>體驗演算法如何讓你上癮</p>
    </div>
    
    <div class="feed" id="feed">
      <!-- Posts will be added here dynamically -->
    </div>
    
    <div class="stats-container">
      <div class="stats-title">演算法分析</div>
      <div class="stat-item">
        <span>個人參與度:</span>
        <span id="engagement-score">0%</span>
      </div>
      <div class="progress-container">
        <div class="progress-bar" id="engagement-bar"></div>
      </div>
      
      <div class="stat-item">
        <span>停留時間:</span>
        <span id="time-spent">0 秒</span>
      </div>
      <div class="progress-container">
        <div class="progress-bar" id="time-bar"></div>
      </div>
      
      <div class="addiction-meter">
        <p>上癮指數: <span id="addiction-level">低</span></p>
      </div>

      <div style="margin-top: 20px;">
        <h4 style="margin-bottom: 10px;">內容偏好圓餅圖</h4>
        <canvas id="interest-chart" width="300" height="300"></canvas>
      </div>
      
    </div>
    
    <div class="controls">
      <button id="refresh-btn">刷新內容</button>
      <button id="reset-btn">重置模擬</button>
    </div>
  </div>
  
  <div class="notification" id="notification">
    <div class="profile">
      <div class="profile-img">!</div>
      <div>
        <div class="name">新通知</div>
        <div class="time">剛剛</div>
      </div>
    </div>
    <div class="content" id="notification-content">
      有新內容等待你查看！
    </div>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/chart.js"></script>
  <script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-datalabels"></script>

  <script>
    // 模擬數據
    // const names = ["Doloris--Ave Mujica","Mortis--Ave Mujica","Timoris--Ave Mujica","Amoris--Ave Mujica","Oblivionis--Ave Mujica","Tomori--MyGo","Anon","Rana","Soyo","Taki"];
    const names = ["Doloris--Ave Mujica","Mortis--Ave Mujica","Timoris--Ave Mujica","Amoris--Ave Mujica","Oblivionis--Ave Mujica","Tomori--MyGo","Anon--MyGo","Rana--MyGo","Soyo--MyGo","Taki--MyGo","Yukina--TOGENASHI","Sayo--TOGENASHI","Lisa--TOGENASHI","Ako--TOGENASHI","Rinko--TOGENASHI",];

    const userTypes = {
      "Doloris--Ave Mujica": "Ave Mujica",
      "Mortis--Ave Mujica": "Ave Mujica",
      "Timoris--Ave Mujica": "Ave Mujica",
      "Amoris--Ave Mujica": "Ave Mujica",
      "Oblivionis--Ave Mujica": "Ave Mujica",
      "Tomori--MyGo": "MyGo",
      "Anon--MyGo": "MyGo",
      "Rana--MyGo": "MyGo",
      "Soyo--MyGo": "MyGo",
      "Taki--MyGo": "MyGo",
      "Yukina--TOGENASHI": "TOGENASHI",
      "Sayo--TOGENASHI": "TOGENASHI",
      "Lisa--TOGENASHI": "TOGENASHI",
      "Ako--TOGENASHI": "TOGENASHI",
      "Rinko--TOGENASHI": "TOGENASHI",
    };

    const contentByType = {
    "Ave Mujica": [
      "命運編織的聲音，今晚也在耳邊迴響。",
      "你也有過逃不掉的黑暗嗎？",
      "無名之歌，是誰的吶喊？",
      "燈光下的我們，是幻影還是真實？",
      "從絕望中誕生的旋律，最動人。"
    ],
    "MyGo": [
      "練團中，今天又吵了一架（笑）",
      "音樂之外，我們還是朋友吧？",
      "第一次的 live，好緊張啊啊啊！",
      "要不要來我們的秘密據點？",
      "就算迷惘，也要彈下去。"
    ],
    "TOGENASHI": [
      "這旋律根本是開場即高潮🔥",
      "我們是透明的火焰。",
      "夜晚的舞台，才是開始。",
      "打破界線，是我們的存在方式。",
      "醒來後的夢，比夢更真。"
    ]
    };


    
    const notifications = [
      "Rikki發布了新貼文！",
      "有人對你的貼文按讚了！",
      "看看這個熱門話題，你可能感興趣！",
      "你錯過了Anon的5則新貼文",
      "你已經有3天沒來查看最新動態了",
      "你竟敢無視燈!!!",
      "有新的朋友請求等待確認",
      "你的貼文獲得了大量關注！",
      "不要錯過今天的熱門話題！"
    ];
    
    const imageUrls = {
      "Ave Mujica": [
        "https://i.imgur.com/UWdolQr.jpeg",
        "https://i.imgur.com/lydaLAn.jpeg",
        "https://i.imgur.com/y07t8cZ.jpeg",
        "https://i.imgur.com/pij1vbc.jpeg",
        "https://i.imgur.com/PFq2HMT.jpeg"
      ],
      "MyGo": [
        "https://i.imgur.com/kIkFYeJ.jpeg",
        "https://i.imgur.com/MNhXALj.jpeg",
        "https://i.imgur.com/ICxnpQi.jpeg",
        "https://i.imgur.com/N2sEW85.jpeg",
        "https://i.imgur.com/8sTUPPQ.jpeg"
      ],
      "TOGENASHI": [
        "https://i.imgur.com/cpt9GIB.jpeg",
        "https://i.imgur.com/xGoMrPq.jpeg",
        "https://i.imgur.com/9lv9QvB.jpeg",
        "https://i.imgur.com/mVFIQLD.jpeg",
        "https://i.imgur.com/zelUeCy.jpeg"
      ]
    };


    // 保存貼文數據的結構
    let postsData = {};
    
    // 保存用戶數據的結構
    let userPosts = {};
    
    // 保存用戶匹配度的結構
    let userEngagement = {};
    
    // 統計數據
    let stats = {
      refreshCount: 0,
      clickCount: 0,
      timeSpent: 0,
      notificationClicks: 0,
      lastRefreshTime: new Date(),
      addictionLevel: "低"
    };
    
    let interestStats = {
      "Ave Mujica": 0,
      "MyGo": 0,
      "TOGENASHI": 0
    };
    
    // 貼文ID計數器
    let postIdCounter = 0;
    
    // 計時器
    let timeCounter;
    let engagementUpdateInterval;
    
    // 停留時間對參與度的影響因子
    const timeEngagementFactor = 0.1;
    
    // 已經使用過的發文者組合追蹤器
    let usedAuthorCombinations = new Set();
    
    // DOM 元素引用
    const feedElement = document.getElementById("feed");
    const notificationElement = document.getElementById("notification");
    const notificationContent = document.getElementById("notification-content");
    const refreshBtn = document.getElementById("refresh-btn");
    const resetBtn = document.getElementById("reset-btn");
    const engagementScore = document.getElementById("engagement-score");
    const engagementBar = document.getElementById("engagement-bar");
    const timeSpentElement = document.getElementById("time-spent");
    const timeBar = document.getElementById("time-bar");
    const addictionLevel = document.getElementById("addiction-level");
    
    // 初始化
    function init() {
      generatePosts(5);
      startTimer();
      startEngagementUpdater();
      scheduleNotifications();
      updateStats();
    }
    
    // 產生貼文
    function generatePosts(count) {
      // 選擇不重複的作者組合
      const selectedAuthors = selectRandomAuthors(count);
      
      // 產生新貼文數據
      for (let i = 0; i < count; i++) {
        createPostData(selectedAuthors[i]);
      }
      
      // 初始化用戶匹配度
      for (const userName of names) {
        if (!userEngagement[userName]) {
          userEngagement[userName] = 0; // 初始匹配度為0
        }
      }
      
      // 排序並顯示貼文
      displaySortedPosts();
    }
    
    // 選擇隨機且每次不同的作者組合
    function selectRandomAuthors(count) {
      // 創建可用作者的副本，以便可以修改它
      let availableAuthors = [...names];
      let selectedAuthors = [];
      
      // 如果作者數量不足，就允許重複
      if (count > availableAuthors.length) {
        for (let i = 0; i < count; i++) {
          const randomIndex = Math.floor(Math.random() * names.length);
          selectedAuthors.push(names[randomIndex]);
        }
      } else {
        // 打亂作者順序
        for (let i = availableAuthors.length - 1; i > 0; i--) {
          const j = Math.floor(Math.random() * (i + 1));
          [availableAuthors[i], availableAuthors[j]] = [availableAuthors[j], availableAuthors[i]];
        }
        
        // 選擇前count個作者
        selectedAuthors = availableAuthors.slice(0, count);
      }
      
      // 記錄此組合
      usedAuthorCombinations.add(selectedAuthors.join('-'));
      
      return selectedAuthors;
    }
    
    // 創建貼文數據
    function createPostData(userName) {
      const postId = "post-" + (postIdCounter++);
      
      // 如果沒有提供用戶名，則隨機選擇
      if (!userName) {
        userName = names[Math.floor(Math.random() * names.length)];
      }
      
      // 獲取該用戶的匹配度，如果沒有則初始化
      if (!userEngagement[userName]) {
        userEngagement[userName] = 0; // 初始匹配度為0
      }
      
      // 生成隨機內容和圖片
      const userType = userTypes[userName] || "Ave Mujica"; // 預設防呆
      const typeContents = contentByType[userType];
      const randomContent = typeContents[Math.floor(Math.random() * typeContents.length)];

      const hasImage = Math.random() > 0.5;
      const imageList = imageUrls[userType] || [];
      const imageUrl = hasImage && imageList.length > 0
        ? imageList[Math.floor(Math.random() * imageList.length)]
        : "";

      // 存儲貼文資料，添加隨機因素
      postsData[postId] = {
        id: postId,
        engagement: userEngagement[userName] + Math.floor(Math.random() * 10), // 添加隨機波動
        name: userName,
        content: randomContent,
        time: Math.floor(Math.random() * 60),
        likes: Math.floor(Math.random() * 20),
        comments: Math.floor(Math.random() * 5),
        hasImage: hasImage,
        imageUrl: imageUrl
      };
      
      // 同時建立用戶-貼文關聯
      if (!userPosts[userName]) {
        userPosts[userName] = [];
      }
      userPosts[userName].push(postId);
      
      return postId;
    }
    
    // 顯示排序後的貼文
    function displaySortedPosts() {
    feedElement.innerHTML = '';

    const sortedPostIds = Object.keys(postsData).sort((a, b) => {
      const postA = postsData[a];
      const postB = postsData[b];

      const randomFactorA = Math.floor(Math.random() * 11) - 5;
      const randomFactorB = Math.floor(Math.random() * 11) - 5;

      const typeA = userTypes[postA.name] || "Ave Mujica";
      const typeB = userTypes[postB.name] || "Ave Mujica";

      const interestBonusA = (interestStats[typeA] || 0) * 2; // 可以調整倍率
      const interestBonusB = (interestStats[typeB] || 0) * 2;

      const scoreA = postA.engagement + interestBonusA + randomFactorA;
      const scoreB = postB.engagement + interestBonusB + randomFactorB;

      return scoreB - scoreA;
    });

    for (const postId of sortedPostIds) {
      const post = createPostElement(postId);
      feedElement.appendChild(post);
    }
  }

    
    // 創建貼文元素
    function createPostElement(postId) {
      const postData = postsData[postId];
      
      const post = document.createElement("div");
      post.className = "post";
      post.id = postId;
      
      const engagementTag = document.createElement("div");
      engagementTag.className = "engagement";
      engagementTag.textContent = `演算法匹配度: ${postData.engagement}%`;
      engagementTag.id = `engagement-${postId}`;
      post.appendChild(engagementTag);
      
      const profile = document.createElement("div");
      profile.className = "profile";
      
      const profileImg = document.createElement("div");
      profileImg.className = "profile-img";
      profileImg.textContent = postData.name.charAt(0);
      
      const info = document.createElement("div");
      const nameElement = document.createElement("div");
      nameElement.className = "name";
      nameElement.textContent = postData.name;
      
      const time = document.createElement("div");
      time.className = "time";
      time.textContent = `${postData.time}分鐘前`;
      
      info.appendChild(nameElement);
      info.appendChild(time);
      profile.appendChild(profileImg);
      profile.appendChild(info);
      post.appendChild(profile);
      
      const content = document.createElement("div");
      content.className = "content";
      content.textContent = postData.content;
      post.appendChild(content);
     
      // 如果有圖片，添加圖片
      if (postData.hasImage) {
        const image = document.createElement("img");
        image.className = "image";
        image.src = postData.imageUrl;
        image.alt = "貼文圖片";
        post.appendChild(image);
      } 
      
      // 互動統計
      const statsDiv = document.createElement("div");
      statsDiv.className = "stats";
      statsDiv.textContent = `${postData.likes} 個讚 · ${postData.comments} 則留言`;
      statsDiv.id = `stats-${postId}`;
      post.appendChild(statsDiv);
      
      // 互動按鈕
      const actions = document.createElement("div");
      actions.className = "actions";

      const likeAction = document.createElement("div");
      likeAction.className = "action";
      likeAction.textContent = "讚";
      likeAction.addEventListener("click", function () {
        stats.clickCount++;
        updatePostEngagement(postId);
        likeAction.style.color = "#4267B2";
        likeAction.style.fontWeight = "bold";

        postData.likes++;
        statsDiv.textContent = `${postData.likes} 個讚 · ${postData.comments} 則留言`;

        // 加權 +1
        interestStats[userTypes[postData.name]] += 1;
        updateInterestChart();
        updateStats();
      });

      const commentAction = document.createElement("div");
      commentAction.className = "action";
      commentAction.textContent = "留言";
      commentAction.addEventListener("click", function () {
        stats.clickCount++;
        updatePostEngagement(postId);
        postData.comments++;
        statsDiv.textContent = `${postData.likes} 個讚 · ${postData.comments} 則留言`;

        // 加權 +1
        interestStats[userTypes[postData.name]] += 1;
        updateInterestChart();
        updateStats();
      });

      const shareAction = document.createElement("div");
      shareAction.className = "action";
      shareAction.textContent = "分享";
      shareAction.addEventListener("click", function () {
        stats.clickCount++;
        updatePostEngagement(postId);

        // 加權 +2
        interestStats[userTypes[postData.name]] += 2;
        updateInterestChart();
        updateStats();
      });

      actions.appendChild(likeAction);
      actions.appendChild(commentAction);
      actions.appendChild(shareAction);
      post.appendChild(actions);
      
      return post;
    }
    
    // 更新貼文及發文者匹配度
    function updatePostEngagement(postId) {
      const post = postsData[postId];
      const userName = post.name;
      
      // 增加匹配度，但最多不超過100%
      const increaseAmount = Math.floor(2 + Math.random() * 5);
      post.engagement = Math.min(100, post.engagement + increaseAmount);
      
      // 同時也增加用戶的匹配度
      userEngagement[userName] = Math.min(100, userEngagement[userName] + increaseAmount);
      
      // 更新該用戶所有貼文的匹配度
      for (const userPostId of userPosts[userName]) {
        postsData[userPostId].engagement = userEngagement[userName];
        
        // 更新顯示
        const engagementTag = document.getElementById(`engagement-${userPostId}`);
        if (engagementTag) {
          engagementTag.textContent = `演算法匹配度: ${userEngagement[userName]}%`;
        }
      }
      
      // 更新顯示
      const engagementTag = document.getElementById(`engagement-${postId}`);
      if (engagementTag) {
        engagementTag.textContent = `演算法匹配度: ${post.engagement}%`;
      }
    }
    
    // 找出中央的貼文
    function findCenterPost() {
      const feed = document.getElementById('feed');
      const feedRect = feed.getBoundingClientRect();
      const feedCenter = feedRect.top + feedRect.height / 2;
      
      let closestPost = null;
      let closestDistance = Infinity;
      
      // 找遍所有貼文，找出最接近中央的
      const posts = document.querySelectorAll('.post');
      for (const post of posts) {
        const postRect = post.getBoundingClientRect();
        const postCenter = postRect.top + postRect.height / 2;
        const distance = Math.abs(feedCenter - postCenter);
        
        if (distance < closestDistance) {
          closestDistance = distance;
          closestPost = post;
        }
      }
      
      return closestPost ? closestPost.id : null;
    }
    
    // 定期增加中央貼文匹配度，但添加隨機因素
    function startEngagementUpdater() {
      engagementUpdateInterval = setInterval(() => {
        // 只有一定機率增加中央貼文匹配度
        if (Math.random() > 0.3) { // 70% 機率
          const centerPostId = findCenterPost();
          if (centerPostId) {
            const post = postsData[centerPostId];
            const userName = post.name;
            
            // 匹配度增加1%
            post.engagement = Math.min(100, post.engagement + 1);
            
            // 同時增加用戶匹配度
            userEngagement[userName] = Math.min(100, userEngagement[userName] + 1);
            
            // 更新該用戶所有貼文的匹配度
            for (const userPostId of userPosts[userName]) {
              postsData[userPostId].engagement = userEngagement[userName];
              
              // 更新顯示
              const engagementTag = document.getElementById(`engagement-${userPostId}`);
              if (engagementTag) {
                engagementTag.textContent = `演算法匹配度: ${userEngagement[userName]}%`;
              }
            }
          }
        }
      }, 1000); // 每秒執行一次
    }
    
    // 顯示通知
    function showNotification() {
      notificationContent.textContent = notifications[Math.floor(Math.random() * notifications.length)];
      notificationElement.style.display = 'block';
      
      // 5秒後自動關閉
      setTimeout(() => {
        notificationElement.style.display = 'none';
      }, 5000);
    }
    
    // 排程通知
    function scheduleNotifications() {
      // 初始延遲
      setTimeout(() => {
        showNotification();
        
        // 之後每隔一段時間顯示通知
        setInterval(() => {
          if (Math.random() > 0.3) { // 70% 機率顯示通知
            showNotification();
          }
        }, 20000 + Math.random() * 30000); // 20-50秒之間隨機
      }, 5000 + Math.random() * 10000); // 5-15秒後顯示第一個通知
    }
    
    // 更新統計數據
    function updateStats() {
      // 根據停留時間增加參與度，同時考慮點擊和刷新
      const timeEngagementContribution = Math.min(50, stats.timeSpent * timeEngagementFactor);
      const userActionsContribution = Math.min(50, (stats.refreshCount * 3 + stats.clickCount * 5 + stats.notificationClicks * 10) / 2);
      
      // 合併兩種參與度來源
      const engagementValue = Math.min(100, Math.floor(timeEngagementContribution + userActionsContribution));
      engagementScore.textContent = `${engagementValue}%`;
      engagementBar.style.width = `${engagementValue}%`;
      
      // 更新時間統計
      timeSpentElement.textContent = `${stats.timeSpent} 秒`;
      const timePercentage = Math.min(100, (stats.timeSpent / 360) * 100); // 6分鐘為100%
      timeBar.style.width = `${timePercentage}%`;
      
      // 計算上癮程度
      if (engagementValue < 30) {
        stats.addictionLevel = "低";
      } else if (engagementValue < 70) {
        stats.addictionLevel = "中";
      } else {
        stats.addictionLevel = "高";
      }
      
      addictionLevel.textContent = stats.addictionLevel;
      
      // 根據上癮程度改變顏色
      if (stats.addictionLevel === "低") {
        addictionLevel.style.color = "green";
      } else if (stats.addictionLevel === "中") {
        addictionLevel.style.color = "orange";
      } else {
        addictionLevel.style.color = "red";
      }
    }
    
    // 刷新按鈕點擊 - 重寫為每次生成新的作者陣列
    refreshBtn.addEventListener("click", function() {
      stats.refreshCount++;
      stats.lastRefreshTime = new Date();
      
      // 清除一些舊的貼文，保持合理數量
      let currentPostIds = Object.keys(postsData);
      if (currentPostIds.length > 10) {
        // 保留最新的一半貼文
        const keepCount = Math.ceil(currentPostIds.length / 2);
        const oldPostIds = currentPostIds.slice(0, currentPostIds.length - keepCount);
        
        // 刪除舊貼文
        for (const oldPostId of oldPostIds) {
          const userName = postsData[oldPostId].name;
          // 從用戶貼文關聯中刪除
          if (userPosts[userName]) {
            userPosts[userName] = userPosts[userName].filter(id => id !== oldPostId);
          }
          // 刪除貼文數據
          delete postsData[oldPostId];
        }
      }
      // 重置興趣統計數據

      // 獲得新的隨機作者組合 (3-5人)
      const newPostCount = 3 + Math.floor(Math.random() * 3);
      const newAuthors = selectRandomAuthors(newPostCount);
      
      // 為每個作者創建新貼文
      for (const author of newAuthors) {
        createPostData(author);
      }
      
      // 重新顯示排序後的貼文
      displaySortedPosts();
      
      updateStats();
    });
    
    // 重置按鈕點擊
    resetBtn.addEventListener("click", function() {
      // 重置統計數據
      stats = {
        refreshCount: 0,
        clickCount: 0,
        timeSpent: 0,
        notificationClicks: 0,
        lastRefreshTime: new Date(),
        addictionLevel: "低"
      };
      // 重置興趣統計數據
interestStats = {
  "Ave Mujica": 0,
  "MyGo": 0,
  "TOGENASHI": 0
};

// 更新圓餅圖顯示
updateInterestChart();   //改了這
      // 重置貼文數據和ID計數器
      postsData = {};
      userPosts = {};
      userEngagement = {}; // 重置用戶匹配度
      usedAuthorCombinations = new Set(); // 重置作者組合記錄
      postIdCounter = 0;
      
      // 清空貼文
      feedElement.innerHTML = '';
      
      // 重新初始化
      generatePosts(5);
      updateStats();
      
      // 重置計時器
      clearInterval(timeCounter);
      clearInterval(engagementUpdateInterval);
      startTimer();
      startEngagementUpdater();
    });
    
    // 通知點擊
    notificationElement.addEventListener("click", function() {
      stats.notificationClicks++;
      notificationElement.style.display = 'none';
      updateStats();
      
      // 點擊通知後自動刷新內容
      refreshBtn.click();
    });
    
    // 計時器
    function startTimer() {
      timeCounter = setInterval(() => {
        stats.timeSpent++;
        updateStats();
      }, 1000);
    }



// 刪除第一個不完整的函數，只保留下面這個完整版本
function initInterestChart() {
  const ctx = document.getElementById("interest-chart").getContext("2d");
  interestChart = new Chart(ctx, {
    type: "doughnut",
    data: {
      labels: ["Ave Mujica", "MyGo", "TOGENASHI"],
      datasets: [{
        data: [0, 0, 0],
        backgroundColor: ["#E680FF", "#66FFE6", "#e67e22"],
        borderWidth: 1
      }]
    },
    options: {
      responsive: false,
      plugins: {
        legend: {
          position: "bottom"
        },
        datalabels: {
          formatter: (value) => value + "%",
          color: "#000000",
          font: {
            weight: 'bold',
            size: 18
          }
        }
      }
    },
    plugins: [ChartDataLabels]
  });
}

    let interestChart;
    Chart.register(ChartDataLabels);
    function initInterestChart() {
      const ctx = document.getElementById("interest-chart").getContext("2d");
      interestChart = new Chart(ctx, {
        type: "doughnut",
        data: {
          labels: ["Ave Mujica", "MyGo", "TOGENASHI"],
          datasets: [{
            data: [0, 0, 0],
            backgroundColor: ["#E680FF", "#66FFE6", "#e67e22"],
            borderWidth: 1
          }]
        },
        options: {
          responsive: false,
          plugins: {
            legend: {
              position: "bottom"
            }
          }
        }
      });
    }

    function updateInterestChart() {
      const total = interestStats["Ave Mujica"] + interestStats["MyGo"] + interestStats["TOGENASHI"];
      
      if (total === 0) {
        // 初始階段沒有資料時顯示 0
        interestChart.data.datasets[0].data = [0, 0, 0];
      } else {
        interestChart.data.datasets[0].data = [
          (interestStats["Ave Mujica"] / total * 100).toFixed(1),
          (interestStats["MyGo"] / total * 100).toFixed(1),
          (interestStats["TOGENASHI"] / total * 100).toFixed(1)
        ];
      }

      interestChart.update();
    }



    // 初始化應用
    init();
    initInterestChart();

  </script>
</body>
</html>
