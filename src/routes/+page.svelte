<script>
    import Icon from '@iconify/svelte';
</script>
<head>
    <meta charset="UTF-8">
    <title>zZNoelZz - Landing</title>
    <style>
        body {
            background-image: url('/ruby.jpg');
            background-repeat: no-repeat;
            background-attachment: fixed;
            background-size: 100% 100%;
        }

        .flex {
            display: flex;
        }

        .flex-col {
            flex-direction: column;
        }

        .flex-row {
            flex-direction: row;
        }

        .center {
            text-align: center;
            align-items: center;
            justify-content: center;
        }

        .pos {
            margin: 15px;
            padding: 40px;
        }

        .font {
            font-family: Lucida Console;
            font-size: 20px;
        }

        icon {
            color: #808080;
            width: 48px;
            height: 48px;
        }
        .color {
            color: aqua;
        }

        .rainbow-text {
            background-image: linear-gradient(to left, violet, indigo, #1a46f5, green, yellow, orange, red);   -webkit-background-clip: text;
            color: transparent;
        }

        .line {
            height:3px;
            width:600px;
            border-width:0px;
            border-radius: 1px;
            background-color: #ec4088;
            animation-name: fade;
            animation-duration: 4s;
            animation-iteration-count: infinite;
        }

        @keyframes fade {
            0%   {background-color:#ec4088}

            50%  {background-color: #52f3df}

            100% {background-color:#ec4088}
        }
        </style>
</head>
<body>
    <div id="root">
        <div class="flex flex-col center pos">
            <div class="flex flex-col center pos">
                <div>
                    <img src="/banner.png" alt="Noel Banner" style="width: full; height: full"/>
                </div>
            </div>
            <div class="flex flex-col center color font" style="font-size:30px">
                <p>
                    Do you
                    <span style ="color: #ec4088; font-size: 30px;"> believe</span>
                    in
                    <span class="rainbow-text">Miracle</span>
                    ?
                </p>
            </div>
            <div class="flex center" style="margin:1px">
                <hr class="line">
            </div>
        </div>
        <div>
            <ul class="flex flex-row center" style="list-style-type: none; gap: 20px">
                <li>
                    <a href="https://www.facebook.com/profile.php?id=100027751118871" target="_blank">
                        <Icon icon="mdi:facebook" color="gray" width="48" height="48" />
                    </a>
                </li>
                <li>
                    <a href="https://twitter.com/zZNoelZz" target="_blank">
                        <Icon icon="icon-park-twotone:big-x" color="gray" width="45" height="45" />
                    </a>
                </li>
                <li>
                    <a href="https://osu.ppy.sh/users/11923881" target="_blank">
                        <Icon icon="simple-icons:osu" color="gray" width="42" height="42" />
                    </a>
                </li>
                <li>
                    <a href="https://steamcommunity.com/profiles/76561199219775134/" target="_blank">
                        <Icon icon="mdi:steam" color="gray" width="48" height="48" />
                    </a>
                </li>
                <li>
                    <a href="https://www.youtube.com/watch?v=ucbx9we6EHk" target="_blank">
                        <Icon icon="mdi:youtube" color="gray" width="48" height="48" />
                    </a>
                </li>
            </ul>
        </div>
    </div>
    <script type="module" src="https://unpkg.com/ionicons@7.1.0/dist/ionicons/ionicons.esm.js"></script>
</body>
