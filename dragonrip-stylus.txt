/* ==UserStyle==
@name           dragonrip.com
@namespace      github.com/openstyles/stylus
@version        1.0.0
@description    A new userstyle
@author         Me
==/UserStyle== */

@-moz-document domain("dragonrip.com") {
   *, :after, :before {
        -webkit-box-sizing: border-box;
        -moz-box-sizing: border-box;
        box-sizing: border-box;
    }

    /* Change game background here to try prevent flickering on page load */
    body, html {
        background:#262626 url('https://i.imgur.com/gnerbEH.jpeg')!important;
        background-image: url('https://i.imgur.com/gnerbEH.jpeg')!important;
        background-size:auto!important;
        background-repeat:repeat!important;
        margin: auto 0px auto 0px !important;
        xscrollbar-color: rgb(62, 62, 62) grey;
	    xscrollbar-width: thin;
    }

    /* Remove logo here to try prevent flickering on page load */
    body > div.logo > img {
        display:none;
    }	
    
    /* Remove navbar to prevent load flickering */
    .navbar {
        display: none !important;
    }
    
    .player {
        height: 58px;
    }
    
    /* Set here to revent load flickering */
    div.logo {
        height: 68px;
        display: flex;
        align-items: center;
        justify-content: center;
    }

    /* Make main bars darker to avoid flickering on page load */
    .player > .bar,
    .player > .bar > .healthbar,
    .player > .bar > .healthbar > .healthbar2{
        background-color: black!important;
    }

    
    /* Change empty vial graphic to more visible icon */
    div[style="background-image:url(/game/images/itemaa/weavialwat.png);"] {
        background-image:url(https://i.imgur.com/mgV2Iyb.png)!important;
        background-repeat:no-repeat;
        background-position:center;
        background-size:contain;
    }

    
    /* Pet explore and pet training elems on right-side bar */
    .burbul> *:nth-child(7) > tbody > tr > td > br ,
    .burbul> *:nth-child(8)  > tbody > tr > td > br
    {
        border:1px solid lime;
        height:0px!important;
        padding:0px!important;
    }

    
    /* ruins menu icon lvl texts */
    div.resurx > span.amoub > b {
        color:white;
        padding:5px;
        text-shadow: 
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black,
            0px 0px 5px black
        ;
    }
    
    /* chat container */
    .chatting {
        xwidth:98vw !important;
    }
    
    /* Margins for playarea contents, margin is removed in dragonrip-toolbar script. */
    /* To prevent resize "flickering" when scripts load and insert elements */
    .veik {
        margin-top: 130px;
    }
    .into {
        margin-top: 120px;
    }
    


}