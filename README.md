# Meshmesh-games
موقع العاب متميز (المطور واحد فقط)<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <title>موقعي الرائع</title>
</head>
<body>
    <h1>مرحبًا بكم في موقعي!</h1>
</body>
</html>

<!DOCTYPE html>
<html lang="ar">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>ألعاب مع إعلانات</title>
    <link href="https://fonts.googleapis.com/css2?family=Roboto:wght@400;500;700&family=Open+Sans:wght@400;600&display=swap" rel="stylesheet">
    <style>
        body {
            font-family: 'Roboto', sans-serif;
            background-color: #f0f2f5;
            color: #333;
            margin: 0;
            padding: 0;
            text-align: center;
        }

        header {
            background-color: #007BFF;
            color: white;
            padding: 15px;
            font-size: 24px;
            font-weight: 700;
        }

        .game-container {
            display: flex;
            flex-wrap: wrap;
            justify-content: center;
            margin-top: 30px;
            gap: 20px;
            padding: 0 20px;
        }

        .game {
            background-color: white;
            border-radius: 8px;
            box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
            overflow: hidden;
            width: 280px;
            transition: transform 0.3s ease-in-out;
        }

        .game:hover {
            transform: translateY(-10px);
        }

        .game img {
            width: 100%;
            height: 180px;
            object-fit: cover;
            transition: transform 0.3s ease-in-out;
        }

        .game img:hover {
            transform: scale(1.05);
        }

        .game-info {
            padding: 15px;
            text-align: right;
        }

        .game-info h2 {
            font-size: 18px;
            margin: 10px 0;
            font-weight: 500;
            color: #007BFF;
        }

        .game-info p {
            font-size: 14px;
            color: #555;
            margin-bottom: 10px;
        }

        .game-info a {
            display: inline-block;
            background-color: #007BFF;
            color: white;
            padding: 10px 20px;
            border-radius: 5px;
            text-decoration: none;
            font-weight: 600;
            transition: background-color 0.3s ease;
        }

        .game-info a:hover {
            background-color: #0056b3;
        }

        .ad-container {
            margin-top: 30px;
            text-align: center;
        }

        nav {
            background-color: #333;
            padding: 10px;
            position: fixed;
            width: 100%;
            top: 0;
            z-index: 100;
        }

        nav ul {
            list-style-type: none;
            padding: 0;
            margin: 0;
            display: flex;
            justify-content: center;
        }

        nav ul li {
            margin: 0 20px;
        }

        nav ul li a {
            color: white;
            text-decoration: none;
            font-size: 18px;
            font-weight: 600;
        }

        nav ul li a:hover {
            text-decoration: underline;
        }

        .content {
            margin-top: 70px;
        }
    </style>
</head>
<body>

    <header>أفضل الألعاب للتحميل</header>

    <nav>
        <ul>
            <li><a href="#">المصمم احمد مشمش</a></li>
            <li><a href="#">الألعاب</a></li>
            <li><a href="#"> 01225007509لو في خطا اتصل بنا</a></li>
        </ul>
    </nav>

    <div class="content">
        <div class="game-container" id="games-container"></div>

        <div class="ad-container">
            <script async src="https://pagead2.googlesyndication.com/pagead/js/adsbygoogle.js"></script>
            <ins class="adsbygoogle"
                 style="display:block; width: 100%; height: 250px;"
                 data-ad-client="ca-pub-xxxxxxxxxxxxxxxx"
                 data-ad-slot="xxxxxxxxxx"
                 data-ad-format="auto"></ins>
            <script>
                (adsbygoogle = window.adsbygoogle || []).push({});
            </script>
        </div>
    </div> <script>
    const games = [
        {
            name: "The Last of Us Part II", platform: "بلايستيشن", 
            image: "https://upload.wikimedia.org/wikipedia/en/4/45/The_Last_of_Us_Part_II_Cover_Art.jpg",
            downloadLink: "https://www.playstation.com/en-us/games/the-last-of-us-part-ii/",
            description: "لعبة مغامرات ونجاة تقدم قصة قوية في عالم ما بعد الكارثة. تتميز بمستوى عالٍ من التفاصيل في العالم المفتوح."
        },
        {
            name: "Red Dead Redemption 2", platform: "كمبيوتر", 
            image: "https://upload.wikimedia.org/wikipedia/en/4/44/Red_Dead_Redemption_II.jpg",
            downloadLink: "https://www.rockstargames.com/reddeadredemption2/",
            description: "لعبة عالم مفتوح تدور أحداثها في الغرب الأمريكي. تتميز بجودة رسومات عالية ونظام لعب مذهل."
        },
        {
            name: "GTA V", platform: "بلايستيشن وكمبيوتر", 
            image: "https://upload.wikimedia.org/wikipedia/en/a/a5/Grand_Theft_Auto_V.png",
            downloadLink: "https://www.rockstargames.com/V/",
            description: "اللعبة الشهيرة التي تتيح لك استكشاف مدينة لوس سانتوس وعالمها المفتوح مع مهام متعددة."
        },
        {
            name: "Fortnite", platform: "موبايل", 
            image: "https://upload.wikimedia.org/wikipedia/en/0/08/Fortnite_Season_6_Key_Art.jpg",
            downloadLink: "https://www.epicgames.com/fortnite/",
            description: "لعبة باتل رويال شهيرة تجمع بين البناء والقتال في أسلوب لعب مبتكر."
        },
        {
            name: "PUBG Mobile", platform: "موبايل", 
            image: "https://upload.wikimedia.org/wikipedia/commons/1/1c/PUBG_Mobile_logo.png",
            downloadLink: "https://www.pubgmobile.com/",
            description: "لعبة باتل رويال على الموبايل، تتميز بأسلوب لعب مثير حيث يتنافس اللاعبون للبقاء على قيد الحياة."
        },
        {
            name: "Blur", platform: "كمبيوتر وبلايستيشن",
            image: "https://upload.wikimedia.org/wikipedia/en/6/61/Blur_%28video_game%29.jpg",
            downloadLink: "https://www.activision.com/games/blur",
            description: "لعبة سباقات حماسية تتميز بمسارات رائعة وسرعة كبيرة."
        },
        {
            name: "GTA San Andreas", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/6/6d/Grand_Theft_Auto_San_Andreas_Cover_Art.jpg",
            downloadLink: "https://www.rockstargames.com/sanandreas/",
            description: "إحدى أفضل ألعاب العالم المفتوح التي تقدم تجربة فريدة في مدينة سان أندرياس."
        },
        {
            name: "GTA Vice City", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/0/04/Grand_Theft_Auto_Vice_City.png",
            downloadLink: "https://www.rockstargames.com/vicecity/",
            description: "اللعبة الشهيرة التي تدور أحداثها في مدينة فاييس سيتي، مستوحاة من مدينة ميامي."
        },
        {
            name: "GTA IV", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/8/8f/Grand_Theft_Auto_IV_cover_art.jpg",
            downloadLink: "https://www.rockstargames.com/iv/",
            description: "لعبة عالم مفتوح تقدم قصة رائعة حول نيكو بيلك."
        },
        {
            name: "PES 2021", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/2/2a/PES_2021_Cover.jpg",
            downloadLink: "https://www.konami.com/wepes/2021/",
            description: "اللعبة التي تقدم محاكاة رياضية لكرة القدم."
        },
        {
            name: "PES 2017", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/f/f2/PES_2017_cover_art.jpg",
            downloadLink: "https://www.konami.com/wepes/2017/",
            description: "واحدة من أفضل إصدارات لعبة PES."
        },
        {
            name: "FIFA 2023", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/7/7c/FIFA_23_Cover.jpg",
            downloadLink: "https://www.ea.com/games/fifa/fifa-23",
            description: "إصدار حديث من لعبة FIFA."
        },
        {
            name: "Euro Truck Simulator 2", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/3/3d/Euro_Truck_Simulator_2_cover.jpg",
            downloadLink: "https://www.eurotrucksimulator2.com/",
            description: "لعبة محاكاة الشاحنات عبر الطرق الأوروبية."
        },
        {
            name: "Need for Speed: Most Wanted", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/d/d6/Need_for_Speed_Most_Wanted_cover.jpg",
            downloadLink: "https://www.ea.com/games/need-for-speed/need-for-speed-most-wanted",
            description: "لعبة سباق حماسية مع محاكاة القيادة."
        },
        {
            name: "Mortal Kombat 11", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/f/f6/Mortal_Kombat_11_cover_art.jpg",
            downloadLink: "https://www.mortalkombat11.com/",
            description: "لعبة قتال مشهورة بشخصياتها الفريدة والمعارك العنيفة."
        },
        // الألعاب الجديدة التي ترغب في إضافتها
        {
            name: "Valorant", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/2/25/Valorant_logo_2020.png",
            downloadLink: "https://playvalorant.com/",
            description: "لعبة تصويب تنافسية من منظور الشخص الأول تتميز بأسلوب لعب مميز."
        },
        {
            name: "Crossfire", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/a/a2/Crossfire_Logo.png",
            downloadLink: "https://www.crossfire.com/",
            description: "لعبة تصويب تكتيكية من منظور الشخص الأول."
        },
        {
            name: "FC 24", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/7/7c/FIFA_23_Cover.jpg", // Placeholder image for FC 24
            downloadLink: "https://www.ea.com/games/fifa/fifa-24", // Placeholder link for FC 24
            description: "اللعبة الجديدة من EA Sports بعد تغيير الاسم من FIFA."
        },
        {
            name: "FC 25", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/7/7c/FIFA_23_Cover.jpg", // Placeholder image for FC 25
            downloadLink: "https://www.ea.com/games/fifa/fifa-25", // Placeholder link for FC 25
            description: "إصدار جديد من سلسلة ألعاب كرة القدم الشهيرة."
        },
        {
            name: "Among Us", platform: "موبايل وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/d/d3/Among_Us_logo.png",
            downloadLink: "https://www.innersloth.com/gameAmongUs.php",
            description: "لعبة جماعية تتمحور حول العمل الجماعي والخيانة."
        },
        {
            name: "World War", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/4/48/World_War_II.jpg",
            downloadLink: "https://www.worldwar-game.com/",
            description: "لعبة استراتيجية تدور في أحداث الحرب العالمية."
        },
        {
            name: "Battlefield", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/9/9c/Battlefield_Logo.png",
            downloadLink: "https://www.ea.com/games/battlefield",
            description: "لعبة تصويب حربية تتميز بحروب ضخمة وأسلحة متنوعة."
        },
        {
            name: "Clash of Clans", platform: "موبايل",
            image: "https://upload.wikimedia.org/wikipedia/en/4/42/Clash_of_Clans_Logo.png",
            downloadLink: "https://supercell.com/en/games/clashofclans/",
            description: "لعبة استراتيجية مشهورة تتطلب بناء وتطوير القرى."
        },
        {
            name: "Crash Bandicoot", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/6/6d/Crash_Bandicoot_logo.png",
            downloadLink: "https://www.crashbandicoot.com/",
            description: "لعبة منصات تركز على مغامرات شخصية كراش بانديكوت."
        },
        {
            name: "IGI 3", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/3/31/Project_IGI_3_logo.png",
            downloadLink: "https://www.igi3.com/",
            description: "لعبة تصويب تكتيكية حيث تلعب كجندي خاص."
        },
        {
            name: "صلاح الدين 1", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/1/19/Kingdom_Come_Deliverance_cover.jpg",
            downloadLink: "https://www.kingdomcomedeliverance.com/",
            description: "لعبة مغامرات وتاريخية تتمحور حول صلاح الدين."
        },
        {
            name: "Combat Task", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/f/fb/Combat_Task_Logo.jpg",
            downloadLink: "https://www.combattask.com/",
            description: "لعبة تكتيكية مركزة على المهام القتالية."
        },
        {
            name: "Crazy Taxi", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/a/a1/Crazy_Taxi_Logo.jpg",
            downloadLink: "https://www.sega.com/games/crazy-taxi",
            description: "لعبة سباق حماسية مع مهمة نقل الركاب."
        },
        {
            name: "Medal of Honor", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/a/af/Medal_of_Honor_Logo.png",
            downloadLink: "https://www.medalofhonor.com/",
            description: "لعبة حربية تقود فيها القوات الخاصة في الحروب الكبرى."
        },
        {
            name: "Desert Storm", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/9/9b/Desert_Storm_logo.jpg",
            downloadLink: "https://www.desertstormgame.com/",
            description: "لعبة تحاكي حرب الخليج وتقدم مهام قتالية متنوعة."
        },
        {
            name: "Total Overdose", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/c/cb/Total_Overdose_cover.jpg",
            downloadLink: "https://www.totaloverdosegame.com/",
            description: "لعبة أكشن مع مشاهد مليئة بالحركة والتشويق."
        },
        {
            name: "Evil West", platform: "كمبيوتر وبلايستيشن",
            image: "https://upload.wikimedia.org/wikipedia/en/5/57/Evil_West_cover_art.jpg",
            downloadLink: "https://www.evilwest.com/",
            description: "لعبة أكشن تدور أحداثها في الغرب الأمريكي مع العديد من الوحوش."
        },
        {
            name: "Evil Dead", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/1/1b/Evil_Dead_The_Game.jpg",
            downloadLink: "https://www.evildeadthegame.com/",
            description: "لعبة رعب تعتمد على أفلام Evil Dead."
        },
        {
            name: "Half Life 2", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/a/a7/Half-Life_2_cover.jpg",
            downloadLink: "https://www.valvesoftware.com/half-life",
            description: "واحدة من أعظم ألعاب التصويب في التاريخ."
        },
        {
            name: "Commandos", platform: "كمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/commons/4/44/Commandos_Game_Logo.jpg",
            downloadLink: "https://www.commandosgame.com/",
            description: "لعبة استراتيجية في الحرب العالمية الثانية."
        },
        {
            name: "Far Cry 2", platform: "كمبيوتر وبلايستيشن",
            image: "https://upload.wikimedia.org/wikipedia/en/e/ec/Far_Cry_2_cover.jpg",
            downloadLink: "https://www.ubisoft.com/games/far-cry",
            description: "لعبة أكشن في عالم مفتوح مليء بالمخاطر."
        },
        {
            name: "Shank 2", platform: "كمبيوتر وبلايستيشن",
            image: "https://upload.wikimedia.org/wikipedia/en/9/90/Shank_2_cover.jpg",
            downloadLink: "https://www.klei.com/games/shank",
            description: "لعبة أكشن مليئة بالقتال والمهام المتنوعة."
        },
        {
            name: "Deep Rock Galactic", platform: "كمبيوتر وبلايستيشن",
            image: "https://upload.wikimedia.org/wikipedia/en/1/1e/Deep_Rock_Galactic_logo.png",
            downloadLink: "https://www.deeprockgalactic.com/",
            description: "لعبة أكشن تعاونية مع غزوات في كهوف كوكبية."
        },
        {
            name: "Battlefield 4", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/2/29/Battlefield_4_Logo.png",
            downloadLink: "https://www.ea.com/games/battlefield/battlefield-4",
            description: "لعبة تصويب من منظور الشخص الأول مع معارك ضخمة."
        },
        {
            name: "Spider-Man", platform: "بلايستيشن",
            image: "https://upload.wikimedia.org/wikipedia/en/5/52/Spider-Man_PS4_cover.jpg",
            downloadLink: "https://www.playstation.com/en-us/games/marvels-spider-man/",
            description: "لعبة أكشن ومغامرات تدور حول شخصية سبايدر مان."
        },
        {
            name: "The Green Lantern", platform: "بلايستيشن",
            image: "https://upload.wikimedia.org/wikipedia/en/d/df/Green_Lantern_The_Game_Cover.jpg",
            downloadLink: "https://www.greenlantern.com/",
            description: "لعبة أكشن تأخذك إلى عالم الأبطال الخارقين."
        },
        {
            name: "Sniper Ghost Warrior", platform: "بلايستيشن وكمبيوتر",
            image: "https://upload.wikimedia.org/wikipedia/en/e/e7/Sniper_Ghost_Warrior_3_cover_art.jpg",
            downloadLink: "https://www.sniperghostwarrior.com/",
            description: "لعبة تصويب تركز على القنص والمهام التكتيكية."
        }
    ];

    const gamesContainer = document.getElementById("games-container");

    games.forEach(game => {
        const gameDiv = document.createElement('div');
        gameDiv.classList.add('game');
        gameDiv.innerHTML = `
            <img src="${game.image}" alt="${game.name}">
            <div class="game-info">
                <h2>${game.name} (${game.platform})</h2>
                <p>${game.description}</p>
                <a href="${game.downloadLink}" target="_blank">زيارة الموقع</a>
            </div>
        `;
        gamesContainer.appendChild(gameDiv);
    });
</script>
