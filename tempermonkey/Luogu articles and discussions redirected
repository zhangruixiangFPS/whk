// ==UserScript==
// @name         洛谷文章和讨论重定向
// @namespace    http://tampermonkey.net/
// @version      1.0
// @description  在页面左下角添加蓝色按钮，点击后根据当前URL跳转到指定地址
// @author       TwT
// @match        *://www.luogu.com.cn/article/*
// @match        *://www.luogu.com/article/*
// @match        *://www.luogu.com.cn/discuss/*
// @match        *://www.luogu.com/discuss/*
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    // 创建按钮样式
    const style = document.createElement('style');
    style.textContent = `
        #redirectButton {
            position: fixed;
            left: 20px;
            bottom: 20px;
            padding: 10px 15px;
            background-color: #4285f4;
            color: white;
            border: none;
            border-radius: 5px;
            cursor: pointer;
            font-size: 14px;
            z-index: 9999;
            box-shadow: 0 2px 5px rgba(0,0,0,0.2);
            transition: background-color 0.3s;
        }
        #redirectButton:hover {
            background-color: #3367d6;
        }
    `;
    document.head.appendChild(style);

    // 创建按钮
    const button = document.createElement('button');
    button.id = 'redirectButton';
    button.textContent = '快速跳转';
    document.body.appendChild(button);

    // 按钮点击事件
    button.addEventListener('click', function() {
        const currentUrl = window.location.href;

        // 处理文章链接
        if (currentUrl.includes('/article/')) {
            const articleId = currentUrl.split('/article/')[1].split('/')[0];
            const newUrl = `https://www.luogu.me/article/${articleId}`;
            window.location.href = newUrl;
        }
        // 处理讨论链接
        else if (currentUrl.includes('/discuss/')) {
            const discussId = currentUrl.split('/discuss/')[1].split('/')[0];
            const newUrl = `https://lglg.top/${discussId}`;
            window.location.href = newUrl;
        }
    });
})();
