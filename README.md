<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, minimum-scale=1, initial-scale=1.0">
    <style>
        * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: "Montserrat", Arial, Helvetica, sans-serif;
    font-size: 13px;
    overflow-x: hidden;
}
header {
    height: 100px;
    background-color: #000;
    color: #ffff;
}
.header {
    max-width: 1140px;
    height: 100px;
    margin: auto;
    display: flex;
    align-items: center;
}
.logo {
    width: 100px;
    height: 100px;
    background-image: url("/awaxpro/assets/css/images/logo.jpg");
    background-size: cover;
    background-position: center;
}
.menu {
    flex: 1;
    display: flex;
    justify-content: flex-end;
}
.menu a {
    text-decoration: none;
    color: #ffff;
    font-weight: 600;
    text-transform: uppercase;
    padding-left: 10px;
    padding-right: 10px;
    display: flex;
    height: 100px;
    align-items: center;
    border-bottom: 5px solid #000000;
}
.menu a:hover, .menu .active a {
    border-bottom: 5px solid #b88a58;
    color: #ccc;
}
.menu ul {
    list-style: none;
    display: flex;
    text-decoration: none;
}
.menu-opener {
    display: none;
}
/*-------main---------*/

.banner {
    height: calc(100vh - 100px);
    background-color: #333;
    background-image: url("/awaxpro/assets/css/images/bg.jpg");
    background-size: cover;
    background-position: top;
    overflow: hidden;
}
.banner .sliders {
    width: 1000vw;
    height: 100%;
}
.banner .slide {
    width: 100vw;
    height: 100%;
    display: inline-block;
    background-color: rgba(0, 0, 0, 0.8)
}
.banner .slidearea {
    flex-direction: column;
    display: flex;
    height: 100%;
    align-items: center;
    color: #ffff;
    justify-content: center;
}
.banner h1, .banner span {
    text-transform: uppercase;
    font-weight: bold;
    font-size: 50px;
}
.banner h2 {
    text-transform: uppercase;
    font-size: 25px;
    margin-top: 15px;
}
.banner span {
    color: #b88a58;
}
.banner a {
    display: block;
    margin-top: 40px;
    text-align: center;
    padding: 10px 30px;
    background-color: #b88a58;
    color: #ffff;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    border-radius: 25px;
}
.banner .sliders-pointers {
    width: 100vw;
    height: 20px;
    position: absolute;
    margin-top: -50px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.banner .pointer {
    width: 15px;
    height: 15px;
    border: 2px solid #b88a58;
    border-radius: 8px;
    margin-left: 5px;
    margin-right: 5px;
    cursor: pointer;
}
.banner .pointer.active {
    background-color: #b88a58;
}
.default {
    width: 100vw;
    padding-top: 50px;
    padding-bottom: 50px;
}
.default .section-title, .default .section-desc {
    text-align: center;
    text-transform: uppercase;
    font-weight: 600;
}
.default .section-desc {
    font-size: 13px;
    color: #ccc;
    margin-top: 10px;
    margin-bottom: 40px;
}
.default .section-title {
    font-size: 20px;
}
.default .section-body {
    margin: auto;
    max-width: 1140px;
}
.default.light {
    background-color: #f7f7f7;
}
.default.light .section-title, .default.light .section-body {
    color: #000;
}
.default.dark {
    background-color: #000;
}
.default.dark .section-title, .default.dark .section-body {
    color: #fff;
}




/*-------css as áreas--------*/


.section-aboutus {
    display: flex;
}
.section-aboutus--left {
    flex: 1;
}
.section-aboutus--right {
    margin-left: 5px;
    width: 500px;
    text-align: center;
}
.section-aboutus--left a {
    display: inline-block;
    margin-top: 40px;
    text-align: center;
    padding: 10px 30px;
    background-color: #b88a58;
    color: #ffff;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    border-radius: 25px;
}
iframe {
    width: 100%;
    box-shadow: 0px 0px 10px #333;
}
.section-aboutus--left p {
    font-size: 14px;
    line-height: 25px;
}


.services {
    display: flex;
}
.services .box {
    flex: 1;
    text-align: center;
    border-right: 1px solid #333;
    padding: 15px;
}
.services .box:first-child {
    border-left: 1px solid #333;
}
.services .box h4 {
    margin-top: 20px;
    text-transform: uppercase;
    font-size: 18px;
}
.services .box p {
    margin-top: 10px;
    font-size: 13px;
    color: #999;
}


.section-projects {
    display: flex;
    flex-direction: column;
    align-items: center;
}
.section-project--filters {
    border: 1px solid #ccc;
    background-color: #eee;
    border-radius: 30px;
    display: inline-block;
    padding: 0px 20px;
}
.section-project--filters ul,
.section-project--filters li {
    list-style: none;
}
.section-project--filters li {
    display: inline-block;
    padding: 10px;
    text-transform: uppercase;
    font-size: 13px;
    border-left: 1px solid #ccc;
    color: #555;
    border-bottom: 3px solid #eee;
    align-items: center;
    cursor: pointer;
}
.section-project--filters li:hover {
    border-bottom: 3px solid #b88a58;
}
.section-project--filters .active {
    border-bottom: 3px solid #b88a58;
}
.section-project--filters li:first-child {
    border-left: none;
}
.button {
    display: inline-block;
    background-color: rgb(178, 135, 86);
    color: rgb(255, 255, 255);
    text-transform: uppercase;
    font-size: 12px;
    font-weight: 600;
    margin-top: 30px;
    text-decoration: none;
    padding: 10px 30px;
    border-radius: 20px;
}

.section-projects .photos {
    width: 100vw;
    max-width: 1140px;
    margin-top: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.section-projects .photo {
    width: 280px;
}
.photo-area {
    margin: 10px;
    width: 260px;
    height: 160px;
    overflow: hidden;
}
.photo-area img {
    width: inherit;
    height: inherit;
}
.photo-info {
    position: absolute;
    background-color: rgba(0, 0, 0, 0.5);
    width: inherit;
    height: inherit;
    display: none;
    justify-content: center;
    align-items: center;
    flex-direction: column;
    color: #fff;
    cursor: pointer;
}
.photo-info h5 {
    font-size: 18px;
    font-weight: 600px;
}

.photo-area:hover .photo-info {
    display: flex;
}
.photos a {
    display: inline-block;
    margin-top: 40px;
    text-align: center;
    padding: 10px 30px;
    background-color: #b88a58;
    color: #ffff;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    border-radius: 25px;
}

.bg-team {
    background-image: url("../css/images/bg.jpg");
    background-size: cover;
    background-position: center;
    padding: 0px;
}
.section-team-area {
    background-color: rgba(0, 0, 0, 0.8);
    padding-top: 50px;
    padding-bottom: 50px;
}
.section-team {
    overflow: hidden;
    max-width: 880px;
    margin: auto;
}
.section-team .sliders {
    width: 1000vw;
    height: 100%;
}
.section-team .slide {
    width: 280px;
    height: 100%;
    display: inline-block;
    background-color: #fff;
    margin-right: 20px;
    min-height: 300px;
}
.section-team .slidearea {
    flex-direction: column;
    display: flex;
    height: 100%;
    align-items: center;
    color: #000;
    justify-content: center;
    padding: 30px;
    cursor: pointer;
}

.section-team-area .sliders-pointers {
    margin-top: 30px;
    height: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.section-team-area .pointer {
    width: 15px;
    height: 15px;
    border: 2px solid #b88a58;
    border-radius: 8px;
    margin-left: 5px;
    margin-right: 5px;
    cursor: pointer;
}
.section-team-area .pointer.active {
    background-color: #b88a58;
}
.section-team-avatar {
    width: 150px;
    height: auto;
}
.section-team-name {
    text-transform: uppercase;
    font-size: 600px;
    font-size: 17px;
    margin-top: 30px;
}
.section-team-role {
    font-size: 14px;
    color: #999;
    margin-top: 5px;
}
.section-team-social {
    display: flex;
    margin-top: 20px;
}
.section-team-social a {
    display: inline-flex;
    justify-content: center;
    align-items: center;
    width: 25px;
    height: 25px;
    background-color: #ccc;
    border-radius: 13px;
    margin-right: 10px;
}
.section-team-social a:hover {
    background-color: #b88a58;
}

/* minha parte */

.client .sliders {
    width: 1000vw;
    height: 100%;
}
.client .slide {
    width: 100vw;
    height: 100%;
    display: inline-block;
}
.client .slidearea {
    flex-direction: column;
    display: flex;
    padding: 50px;
    align-items: center;
    background-color: #e9e9e9;
    justify-content: center;
    color: #7e7e7e;
}
.client .slidearea p {
    padding-bottom: 60px;
    padding-top: 60px;
    max-width: 900px;
    flex-wrap: wrap;
    font-size: 15px;
}
.client .title, .client h5 {
    color:#000;
    font-weight: 600;
    text-transform: uppercase;
    font-size: 20px;
    padding-top: 20px;
    padding-bottom: 10px;
}
.client h6 {
    color:#000;
    font-size: 15px;
}
.client .desc {
    font-size: 13px;
    color: #ccc;
    margin-top: 10px;
    margin-bottom: 40px;
    text-align: center;
    text-transform: uppercase;
    font-weight: 600;
}

.client a {
    display: block;
    margin-top: 40px;
    text-align: center;
    padding: 10px 30px;
    background-color: #b88a58;
    color: #ffff;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    border-radius: 25px;
}
.client .sliders-pointers {
    width: 100vw;
    height: 20px;
    position: absolute;
    margin-top: -50px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.client .pointer {
    width: 15px;
    height: 15px;
    border: 2px solid #b88a58;
    border-radius: 8px;
    margin-left: 5px;
    margin-right: 5px;
    cursor: pointer;
}
.client .pointer.active {
    background-color: #b88a58;
}

.marcas {
    position: relative;
    background-color: #ffffff;
    display: flex;
    border-top: 1px solid #999;
    box-shadow: 1px 1px 5px 0px #999;
    width: 100vw;
    height: auto;
}
.marcas .box-marca {
    display: flex;
    margin: auto;
    justify-content: center;
    padding: 40px;
}
.marcas .box-marcas {
    flex: 1;
    display: flex;
    max-width: 1140px;
    margin: auto;
    flex-wrap: wrap;
}
.price {
    display: flex;
    flex-direction: column;
    align-items: center;
    background-color: #e9e9e9;
}
.price .title {
    color:#000;
    font-weight: 600;
    text-transform: uppercase;
    font-size: 20px;
    padding-top: 20px;
    padding-bottom: 10px;
}
.price .desc {
    font-size: 13px;
    color: #ccc;
    margin-top: 10px;
    margin-bottom: 40px;
    text-transform: uppercase;
    font-weight: 600;
}
.price-body {
    display: flex;
    flex-wrap: wrap;
    max-width: 1140px;
    margin: auto;
}
.price-boxes {
    background-color: #ffff;
    display: flex;
    flex-direction: column;
    margin-right: 20px;
    justify-content: center;
    align-items: center;
    width: 280px;
    height: auto;
    flex: 1;
}
.price h3, .price h2, .price h4 {
    text-transform: uppercase;
    margin-bottom: 15px;
}
.price h3 {
    font-size: 17px;
    margin-top: 20px;
}
.price h2 {
    font-weight: bold;
    font-size: 40px;
    margin-bottom: 0;
}
.price h4 {
    color: #b8b8b8;
}
.price p {
    margin-bottom: 10px;
    color: #8d8d8d;
}
.price a {
    text-transform: uppercase;
    font-weight: bold;
    font-size: 15px;
    text-decoration: none;
    color: #fff;
    background-color: #373737;
    padding: 15px;
    border-radius: 20px;
    margin-bottom: 20px;
}
.price a:hover {
    background-color: #b88a58
}
.price-body {
    padding-bottom: 50px;
}

.premium .section-body {
    max-width: initial;
}
.section-premium {
    overflow: hidden;
}
.section-premium .sliders {
    width: 1000vw;
    height: 100%;
}
.section-premium .slide {
    width: 100vw;
    height: 100%;
    display: inline-block;
}
.section-premium .slidearea {
    display: flex;
    height: 100%;
    justify-content: center;
    align-items: center;
    max-width: 1140px;
    border-bottom: 1px solid #CCC;
    margin: auto;
    padding-bottom: 40px;
}
.section-premium--left {
    flex: 1;
    text-align: right;
}
.section-premium--left img {
    width: 300px;
    margin-right: 30px;
}
.section-premium--right {
    flex: 1;
}
.section-premium--item {
    display: flex;
    margin-bottom: 20px;
}
.section-premium--left img {
    width: 300px;
    margin-right: 30px;
}
.section-premium--item img {
    width: 20px;
    height: 20px;
    margin-right: 20px;
}
.section-premium--item div {
    flex: 1;
    color: #999;
    line-height: 20px;
}
.section-premium--item div h4 {
    color: #000;
    font-size: 17px;
    font-weight: 600;
}

.section-premium .sliders-pointers {
    width: 100vw;
    height: 20px;
    display: flex;
    justify-content: center;
    align-items: center;
    margin-top: 40px;
}
.section-premium .pointer.active {
    background-color: #B28756;
}
.section-premium .pointer {
    width: 15px;
    height: 15px;
    border: 2px solid #B28756;
    border-radius: 8px;
    margin-left: 5px;
    margin-right: 5px;
    cursor: pointer;
}
.premium a {
    width: 200px;
    display: block;
    margin-top: 40px;
    text-align: center;
    padding: 10px 30px;
    background-color: #b88a58;
    color: #ffff;
    text-decoration: none;
    text-transform: uppercase;
    font-weight: bold;
    border-radius: 25px;
}
.premium .b {
    display: flex;
    justify-content: center;
}



.some-facts {
    display: flex;
}
.some-facts .box {
    flex: 1;
    text-align: center;
    padding: 15px;
    display: flex;
    flex-direction: column;
    align-items: center;
}
.some-facts .box h4 {
    margin-top: 20px;
    text-transform: uppercase;
    font-size: 18px;
}
.some-facts .box p {
    margin-top: 10px;
    font-size: 13px;
    color: #999;
}
.some-facts .box h1 {
    text-transform: uppercase;
    font-size: 50px;
    color: #b88a58;
}
.some-facts .ba {
    width: 20px;
    height: 3px;
    background-color: #999;
}

.redes {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 100vw;
    height: auto;padding: 20px;
    background: #000;
}
.redes .icons {
    display: flex;
    max-width: 1440px;
    color: #999;
    align-items: center;
    justify-content: center;
}
.icons .icons-redes {
    display: flex;
    cursor: pointer;
}
.redes .icons img,
.redes .icons h2 {
    margin-right: 10px;
}


.contact {
    max-width: 450px;
    margin: auto;
    text-align: center;
}
.name-mail {
    display: flex;
}
.name-mail input,
.subject input {
    display: block;
    width: 100%;
    border: none;
    outline: none;
    border-bottom: 1px solid #999;
    padding: 10px;
    height: 40px;
    background-color: #f7f7f7;
}
.name-mail input:first-child {
    margin-right: 20px;
}
.subject input {
    width: 100%;
}
form textarea {
    width: 100%;
    height: 100px;
    resize: none;
    border: none;
    background-color: #f7f7f7;
    outline: none;
    border-bottom: 1px solid #999;
}

form .button {
    display: inline-block;
    background-color: #B28756;
    color: #FFF;
    text-transform: uppercase;
    font-size: 12px;
    font-weight: 600;
    text-decoration: none;
    padding: 10px 30px;
    margin-top: 30px;
    border-radius: 20px;
}
.map {
    background-image: url("/awaxpro/assets/css/images/mapa.jpg");
    background-size: cover;
    background-position: center;
    padding-top: 30px;
    padding-bottom: 30px;
}
.section-map-area {
    max-width: 1140px;
    margin: auto;
}
.section-map-info {
    width: 50%;
    padding: 30px;
    background-color: #fff;
    color: #000;
}
.section-map-info-item {
    display: flex;
    align-items: center;
    color: #999;
    margin-bottom: 10px;
}
.section-map-info-item-img {
    width: 30px;
    height: 30px;
    display: inline-flex;
    justify-content: center;
    align-items: center;
    padding: 5px;
    background-color: #999;
    border-radius: 15px;
    margin-right: 15px;
}
.section-map-info-item-img img {
    width: 15px;
    height: auto;
}
footer {
    background-color: #000;
}
.footer-area {
    display: flex;
    max-width: 1140px;
    margin: auto;
}
.footer-box, .footer-box2, .footer-box3 {
    flex: 1;
    display: flex;
    color: #999;
    justify-content: start;
    align-items: flex-start;
}
.footer-box {
    padding-top: 30px;
    padding-bottom: 30px;
}
.footer-img {
    display: inline-flex;
    width: 25px;
    height: 25px;
    background-color: #333;
    border-radius: 15px;
    align-items: center;
    justify-content: center;
    margin-right: 10px;
    cursor: pointer;
}
.footer-img:hover {
    background-color: #b88a58;
}
.footer-img img {
    width: 10px;
    height: auto;
}
.footer-box2 {
    margin-top: 20px;
    padding: 0px 10px 10px;
    font-size: 13px;
    line-height: 20px;
}
.footer-box3 {
    padding: 0px;
    margin: 0px;
    display: flex;
    flex-direction: column;
    background-color: #333;
    align-items: center;
    justify-content: center;
    margin-bottom: 20px;
    margin-top: 20px;
}
.footer-box3 form {
    text-align: center;
    padding: 30px;
    display: inline-block;
}
.footer-box3 form input[type=text] {
    background-color: transparent;
    border: none;
    border-bottom: 1px solid #fff;
    width: 100%;
    height: 40px;
    outline: none;
}

/*responsividade*/

@media (min-width: 450px) and (max-width: 800px) {
    .menu-opener {
        display: block;
        width: 45px;
        margin-right: 30px;
    }
    nav {
        display: none;
        position: absolute;
        z-index: 99;
        background-color: rgba(0, 0, 0, 0.9);
        width: 70%;
        height: calc(100vh - 100px);
        top: 100px;
        right: 0;
    }
    .menu ul {
        flex-direction: column;
    }
    .menu li a {
        font-weight: bold;
        height: 80px;
        font-size: 27px;
        margin-left: 50px;
        border: 0;
    }
    .menu li.active a {
        border: 0; 
        color: #b88a58;
    }
    .logo {
        margin-left: 30px;
    }
    .section-aboutus {
        flex-direction: column;
        align-items: center;
    }
    .section-aboutus--left {
        text-align: center;
        padding-bottom: 10px;
    }
    .services {
        flex-wrap: wrap;
    }
    .services .box {
        min-width: 50%;
    }
    .services:first-child {
        border: none;
    }
    .section-team {
        max-width: 580px;
    }
    .price-body {
        flex-direction: column;
    }
    .price-boxes:nth-child(odd) {
        background-color: #CCC;
    }
    .price-boxes {
        width: 100vw;
    }
    .section-premium .slidearea {
        flex-direction: column;
    }
    .section-premium--right {
        padding: 50px;
    }
    .some-facts {
        flex-wrap: wrap;
    }
    .some-facts .box {
        min-width: 50%;
    }
    .section-map-area, .section-map-info {
        width: auto;
    }
    
}




@media (max-width: 450px) {
    .menu-opener {
        display: block;
        width: 45px;
        margin-right: 30px;
    }
    nav {
        display: none;
        position: absolute;
        z-index: 99;
        background-color: rgba(0, 0, 0, 0.9);
        width: 80%;
        height: calc(100vh - 100px);
        top: 100px;
        right: 0;
    }
    .menu ul {
        flex-direction: column;
    }
    .menu li a {
        font-weight: bold;
        height: 60px;
        font-size: 20px;
        margin-left: 30px;
        border: 0;
    }
    .menu li.active a {
        border: 0; 
        color: #b88a58;
    }

    .banner h1, .banner span {
        font-size: 30px;
        text-align: center;
    }
    .banner h2 {
        font-size: 15px;
    }

    .logo {
        margin-left: 30px;
    }
    .section-aboutus {
        flex-direction: column;
        align-items: center;
    }
    .section-aboutus--left {
        text-align: center;
        padding-bottom: 10px;
    }
    .section-aboutus--right {
        width: auto;
        margin-left: 30px;
        margin-right: 30px;
    }
    .section-aboutus--right iframe {
        width: 100%;
        height: auto;
    }
    .services {
        flex-wrap: wrap;
    }
    .services .box {
        min-width: 100%;
    }
    .services:first-child {
        border: none;
    }
    .section-project--filters {
        margin-left: 30px;
        margin-right: 30px;
    }
    .section-team {
        max-width: 280px;
    }
    .price-body {
        flex-direction: column;
    }
    .price-boxes:nth-child(odd) {
        background-color: #CCC;
    }
    .price-boxes {
        width: 100vw;
    }
    .section-premium .slidearea {
        flex-direction: column;
    }
    .section-premium--right {
        padding: 50px;
    }
    .some-facts {
        flex-wrap: wrap;
    }
    .some-facts .box {
        min-width: 100%;
    }
    .redes {
        display: none;
    }
    .contact {
        max-width: 350px;
    }
    .section-map-area, .section-map-info {
        width: auto;
    }
    .section-map-area {
        padding: 0px;
        padding-bottom: 250px;
    }
    

    .footer-area {
        flex-direction: column;
    }
    .footer-box {
        justify-content: center;
    }
}
    </style>
    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,100;0,300;0,400;0,600;0,700;1,300;1,400;1,600;1,700&family=Pacifico&display=swap" rel="stylesheet">
    <title>Awax</title>
</head>
<body>
    <header>
        <div class="header">
            <div class="logo"></div>
            <div class="menu">
                <img class="menu-opener" src="/awaxpro/assets/css/images/menu.png" alt="">
                <nav>
                    <ul>
                        <li class="active"><a href="">Home</a></li>
                        <li><a href="">About Us</a></li>
                        <li><a href="">Services</a></li>
                        <li><a href="">Our Projects</a></li>
                        <li><a href="">Our Team</a></li>
                        <li><a href="">Happy Clients</a></li>
                        <li><a href="">Price</a></li>
                        <li><a href="">Some Facts</a></li>
                        <li><a href="">Contact Us</a></li>
                    </ul>
                </nav>
            </div>
        </div>
    </header>
    <main>
        <section class="banner">
            <div class="sliders">
                <div class="slide">
                    <div class="slidearea">
                        <h1>Design is about<br/><span>Communication</span></h1>
                        <h2>Call Us: +00 0 1234 5678</h2>
                        <a href="">get in touch!</a>
                    </div>
                </div>
                <div class="slide">
                    ...2
                </div>
                <div class="slide">
                    ...3
                </div>
            </div>
            <div class="sliders-pointers">
                <div class="pointer active"></div>
                <div class="pointer"></div>
                <div class="pointer"></div>
            </div>
        </section>

        <section class="default light">
            <div class="section-title">About us</div>
            <div class="section-desc">Who we are?</div>
            <div class="section-body">
                <div class="section-aboutus">
                    <div class="section-aboutus--left">
                        <p>ipsum dolor sit, amet consectetur adipisicing elit. Animi odit commodi assumenda maiores eveniet error labore, tempora accusamus illo voluptates, dolorum quos suscipit corrupti, voluptatum laudantium culpa ipsam. Libero, unde!
                            Lorem ipsum dolor sit amet consectetur, adipisicing elit. Ab deserunt iusto ad architecto esse voluptates neque, ducimus eaque cupiditate blanditiis voluptatibus? Illo ullam perferendis voluptas delectus saepe, molestiae sint nisi?</p> 

                        <a href="">Lern More</a>
                    </div>
                    <div class="section-aboutus--right">
                        <iframe width="560" height="315" src="https://www.youtube.com/embed/oINPn8VjexU" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
                    </div>
                </div>
            </div>
        </section>

        <section class="default dark">
            <div class="section-title">Services</div>
            <div class="section-desc">Services that we provide</div>
            <div class="section-body">
                <div class="services">
                    <div class="box">
                        <img src="/awaxpro/assets/css/images/medalha.png" alt="">
                        <h4>High Quality Design</h4>
                        <p>Um site responsivo</p>
                    </div>
                    <div class="box">
                        <img src="/awaxpro/assets/css/images/estrela.png" alt="">
                        <h4>Modern Design</h4>
                        <p>Um site responsivo</p>
                    </div>
                    <div class="box">
                        <img src="/awaxpro/assets/css/images/relogio.png" alt="">
                        <h4>Regular Updates</h4>
                        <p>Um site responsivo</p>
                    </div>
                    <div class="box">
                        <img src="/awaxpro/assets/css/images/balao.png" alt="">
                        <h4>Fast and Free Support</h4>
                        <p>Um site responsivo</p>
                    </div>
                </div>
            </div>
        </section>

        <section class="default light">
            <div class="section-title">our projects</div>
            <div class="section-desc">what we create</div>
            <div class="section-body">
               <div class="section-projects">
                <div class="section-project--filters">
                    <ul>
                        <li>All</li>
                        <li class="active">photos</li>
                        <li>branding</li>
                        <li>adverts</li>
                        <li>development</li>
                        <li>misc</li>
                    </ul>
                </div>
                <div class="photos">
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto1.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto2.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto3.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto4.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto5.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto6.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto1.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto2.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto3.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto4.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto5.jpg" alt="">
                        </div>
                    </div>
                    <div class="photo">
                        <div class="photo-area">
                            <div class="photo-info">
                                <h5>ABOUT</h5>
                                <p>Aenean a posuere magna, id volutpat.</p>
                            </div>
                            <img src="media/foto6.jpg" alt="">
                        </div>
                    </div>
                </div>
                <a href="" class="button">more projects</a>
               </div>
            </div>
        </section>

<section class="default dark bg-team">
    <div class="section-team-area">
        <div class="section-title">our team</div>
        <div class="section-desc">our co-workers</div>
        <div class="section-team">
            <div class="sliders">
                <div class="slide">
                    <div class="slidearea">
                        <img class="section-team-avatar" src="media/mulher1.png" alt="">
                                <div class="section-team-name">Jane Doe</div>
                                <div class="section-team-role">Master mind</div>
                                <div class="section-team-social">
                                    <a href=""><img src="assets/css/images/facebook.png" alt=""></a>
                                    <a href=""><img src="assets/css/images/googleplus.png" alt=""></a>
                                    <a href=""><img src="assets/css/images/linkedin.png" alt=""></a>
                                    <a href=""><img src="assets/css/images/pinterest.png" alt=""></a>
                                    <a href=""><img src="assets/css/images/twitter.png" alt=""></a>
                                </div>
                    </div>
                </div>
                <div class="slide">
                    <div class="slidearea">
                        <img class="section-team-avatar" src="media/homem1.png" alt="">
                        <div class="section-team-name">Mike shiller</div>
                        <div class="section-team-role">creative head</div>
                        <div class="section-team-social">
                            <a href=""><img src="assets/css/images/facebook.png" alt=""></a>
                            <a href=""><img src="assets/css/images/googleplus.png" alt=""></a>
                            <a href=""><img src="assets/css/images/linkedin.png" alt=""></a>
                            <a href=""><img src="assets/css/images/pinterest.png" alt=""></a>
                            <a href=""><img src="assets/css/images/twitter.png" alt=""></a>
                        </div>
                    </div>
                </div>
                <div class="slide">
                    <div class="slidearea">
                        <img class="section-team-avatar" src="media/mulher2.png" alt="">
                        <div class="section-team-name">anna johns</div>
                        <div class="section-team-role">technical lead</div>
                        <div class="section-team-social">
                            <a href=""><img src="assets/css/images/facebook.png" alt=""></a>
                            <a href=""><img src="assets/css/images/googleplus.png" alt=""></a>
                            <a href=""><img src="assets/css/images/linkedin.png" alt=""></a>
                            <a href=""><img src="assets/css/images/pinterest.png" alt=""></a>
                            <a href=""><img src="assets/css/images/twitter.png" alt=""></a>
                        </div>
                    </div>
                </div>
                <div class="slide">
                    <div class="slidearea">
                        <img class="section-team-avatar" src="media/mulher2.png" alt="">
                        <div class="section-team-name">Hadna Leão</div>
                        <div class="section-team-role">recursos humanos</div>
                        <div class="section-team-social">
                            <a href=""><img src="assets/css/images/facebook.png" alt=""></a>
                            <a href=""><img src="assets/css/images/googleplus.png" alt=""></a>
                            <a href=""><img src="assets/css/images/linkedin.png" alt=""></a>
                            <a href=""><img src="assets/css/images/pinterest.png" alt=""></a>
                            <a href=""><img src="assets/css/images/twitter.png" alt=""></a>
                        </div>
                    </div>
                </div>
            </div>
        </div>
        <div class="sliders-pointers">
            <div class="pointer active"></div>
            <div class="pointer"></div>
            <div class="pointer"></div>
        </div>
    </div>
</section>

<section class="client">
    <div class="sliders">
        <div class="slide">
            <div class="slidearea">
                <div class="title">Happy Clients</div>
                <div class="desc">client reviews</div>
                <img src="/awaxpro/media/homem2.png" alt="">
                <h5>John Done</h5>
                <h6>Head of PR Departament</h6>
                <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Est totam dolores aliquam illo eveniet suscipit nihil quam! Totam voluptatibus nostrum ex fugiat temporibus aspernatur, tempore in consectetur, fugit, qui culpa!</p>
            </div>
        </div>
        <div class="slide">
            ...2
        </div>
        <div class="slide">
            ...3
        </div>
    </div>
    <div class="sliders-pointers">
        <div class="pointer active"></div>
        <div class="pointer"></div>
        <div class="pointer"></div>
    </div>
</section>

<section class="marcas">
    <div class="box-marcas">
        <div class="box-marca">
            <img src="/awaxpro/media/empresa1.png" alt="">
        </div>
        <div class="box-marca">
            <img src="/awaxpro/media/empresa2.png" alt="">
        </div>
        <div class="box-marca">
            <img src="/awaxpro/media/empresa3.png" alt="">
        </div>
        <div class="box-marca">
            <img src="/awaxpro/media/empresa4.png" alt="">
        </div>
        <div class="box-marca">
            <img src="/awaxpro/media/empresa5.png" alt="">
        </div>
        <div class="box-marca">
            <img src="/awaxpro/media/empresa6.png" alt="">
        </div>
    </div>
</section>

<section class="price">
    <div class="title">Happy Clients</div>
    <div class="desc">client reviews</div>
    <div class="price-body">
        <div class="price-boxes">
            <h3>express</h3>
            <h2>$ 9.99</h2>
            <h4>/MONTH</h4>
            <p>Tracking Issues</p>
            <p>Add bugs though email</p>
            <p>Notifications</p>
            <p>Time tracking</p>
            <p>Custom views</p>
            <a href="">choose</a>
        </div>
        <div class="price-boxes">
            <h3>express</h3>
            <h2>$ 9.99</h2>
            <h4>/MONTH</h4>
            <p>Tracking Issues</p>
            <p>Add bugs though email</p>
            <p>Notifications</p>
            <p>Time tracking</p>
            <p>Custom views</p>
            <a href="">choose</a>
        </div>
        <div class="price-boxes">
            <h3>express</h3>
            <h2>$ 9.99</h2>
            <h4>/MONTH</h4>
            <p>Tracking Issues</p>
            <p>Add bugs though email</p>
            <p>Notifications</p>
            <p>Time tracking</p>
            <p>Custom views</p>
            <a href="">choose</a>
        </div>
        <div class="price-boxes">
            <h3>express</h3>
            <h2>$ 9.99</h2>
            <h4>/MONTH</h4>
            <p>Tracking Issues</p>
            <p>Add bugs though email</p>
            <p>Notifications</p>
            <p>Time tracking</p>
            <p>Custom views</p>
            <a href="">choose</a>
        </div>
    </div>
</section>

<section class="default light premium">
    <div class="section-title">Premium</div>
    <div class="section-desc">Even More Features Available</div>
    <div class="section-body">
        <div class="section-premium">
            <div class="sliders" style="margin-left:0;">
                <div class="slide">
                    <div class="slidearea">
                        <div class="section-premium--left">
                            <img src="media/livros.png" />
                        </div>
                        <div class="section-premium--right">
                                <div class="section-premium--item">
                                    <img src="/awaxpro/assets/css/images/check.png" />
                                    <div>
                                        <h4>FIRST FEATURE</h4>
                                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vel eros vitae erat condimentum viverra a nec lacus.<br/>
                                        -- FEATURE ONE<br/>
                                        -- FEATURE TWO<br/>
                                        -- FEATURE THREE
                                    </div>
                                </div>
                                <div class="section-premium--item">
                                    <img src="/awaxpro/assets/css/images/check.png" />
                                    <div>
                                        <h4>SECOND FEATURE</h4>
                                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vel eros vitae erat condimentum viverra a nec lacus.
                                    </div>
                                </div>
                                <div class="section-premium--item">
                                    <img src="/awaxpro/assets/css/images/check.png" />
                                    <div>
                                        <h4>THIRD FEATURE</h4>
                                        Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vel eros vitae erat condimentum viverra a nec lacus.
                                    </div>
                                </div>
                        </div>
                    </div>
                </div><div class="slide">
                    <div class="slidearea">
                        ...
                    </div>
                </div><div class="slide">
                    <div class="slidearea">
                        ...
                    </div>
                </div>
            </div>
            <div class="sliders-pointers">
                <div class="pointer active"></div>
                <div class="pointer"></div>
                <div class="pointer"></div>
            </div>
        </div>
    </div>
    <div class="b">
        <a href="">get in touch</a>
    </div>
</section>

<section class="default dark">
    <div class="section-title">some facts</div>
    <div class="section-desc">about our work</div>
    <div class="section-body">
        <div class="some-facts">
            <div class="box">
                <h1>1000</h1>
                <div class="ba"></div>
                <h4>design projects Released</h4>
                <p>Um site responsivo</p>
            </div>
            <div class="box">
                <h1>900</h1>
                <div class="ba"></div>
                <h4>photos</h4>
                <p>Um site responsivo</p>
            </div>
            <div class="box">
                <h1>500</h1>
                <div class="ba"></div>
                <h4>marketing ideas</h4>
                <p>Um site responsivo</p>
            </div>
            <div class="box">
                <h1>100</h1>
                <div class="ba"></div>
                <h4>Exhibitions</h4>
                <p>Um site responsivo</p>
            </div>
        </div>
    </div>
</section>

<section class="redes">
    <div class="icons">
        <img src="/awaxpro/assets/css/images/share.png" alt="">
        <h2>Tell About Us:</h2>
        <div class="icons-redes">
            <img src="/awaxpro/assets/css/images/twitter.png" alt="">
            <h2>130</h2>
        </div>
        <div class="icons-redes">
            <img src="/awaxpro/assets/css/images/linkedin.png" alt="">
            <h2>130</h2>
        </div>
        <div class="icons-redes">
            <img src="/awaxpro/assets/css/images/facebook.png" alt="">
            <h2>130</h2>
        </div>
        <div class="icons-redes">
            <img src="/awaxpro/assets/css/images/googleplus.png" alt="">
            <h2>130</h2>
        </div>
        <div class="icons-redes">
            <img src="/awaxpro/assets/css/images/pinterest.png" alt="">
            <h2>130</h2>
        </div>
    </div>
</section>

<section class="default light">
    <div class="section-title">CONTACT US</div>
    <div class="section-desc">OUR AGENCY LOCATED IN MELBOURNE, AUSTRALIA</div>
    <div class="section-body">
        <div class="contact">
            <form action="" method="post">
                <div class="name-mail">
                    <input type="text" name="" id="" placeholder="NAME">
                    <input type="text" name="" id="" placeholder="EMAIL">
                </div>
                <div class="subject">
                    <input type="search" name="" id="" placeholder="SUBJECT">
                    <textarea name="message" placeholder="MESSAGE"></textarea>
                </div>
                <input type="submit" value="SEND MESSAGE" class="button">
            </form>
        </div>
    </div>
</section>

<section class="map">
    <div class="section-map-area">
        <div class="section-map-info">
            <div class="section-map-info-item">
                <div class="section-map-info-item-img">
                    <img src="/awaxpro/assets/css/images/carta.png" alt="">
                </div>
                Endereço completão que irá ter algum tamanho
            </div>
            <div class="section-map-info-item">
                <div class="section-map-info-item-img">
                    <img src="/awaxpro/assets/css/images/localizacao.png" alt="">
                </div>
                Endereço completão que irá ter algum tamanho
            </div>
            <div class="section-map-info-item">
                <div class="section-map-info-item-img">
                    <img src="/awaxpro/assets/css/images/telefone.png" alt="">
                </div>
                Endereço completão que irá ter algum tamanho
            </div>
            <div class="section-map-info-item">
                <div class="section-map-info-item-img">
                    <img src="/awaxpro/assets/css/images/arroba.png" alt="">
                </div>
                Endereço completão que irá ter algum tamanho
            </div>
            <div class="section-map-info-item">
                <div class="section-map-info-item-img">
                    <img src="/awaxpro/assets/css/images/web.png" alt="">
                </div>
                Endereço completão que irá ter algum tamanho
            </div>
        </div>
    </div>
</section>

    </main>
    <footer>
        <div class="footer-area">
            <div class="footer-box">
                <div class="footer-img">
                    <img src="/awaxpro/assets/css/images/twitter.png" alt="">
                </div>
                <div class="footer-img">
                    <img src="/awaxpro/assets/css/images/linkedin.png" alt="">
                </div>
                <div class="footer-img">
                    <img src="/awaxpro/assets/css/images/facebook.png" alt="">
                </div>
                <div class="footer-img">
                    <img src="/awaxpro/assets/css/images/googleplus.png" alt="">
                </div>
                <div class="footer-img">
                    <img src="/awaxpro/assets/css/images/pinterest.png" alt="">
                </div>
            </div>
            <div class="footer-box2">
                Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed vel eros vitae erat condimentum viverra a nec lacus. Maecenas eros lectus, rhoncus vel dictum vel, dignissim eget ligula. Vestibulum id tempus quam, sed pellentesque quam. Vestibulum porta aliquet risus, ac rhoncus sem aliquet ac. Donec tincidunt cursus elit vitae euismod.
            </div>
            <div class="footer-box3">
                <form action="" method="post">
                    <input type="text" name="" id="" placeholder="EMAIL TO SUBSCRIBE">
                    <div class="sub">
                        <input type="submit" value="SUBSCRIBE" class="button">
                    </div>
                </form>
            </div>
        </div>
    </footer>
</body>
</html>
