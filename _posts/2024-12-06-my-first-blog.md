---
layout: post
title: "冲"
date: 2024-12-06
categories: [月建, blank]
tags: [NO,NO ]
---
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>文章目录示例</title>
    <style>
        /* 页面布局 */
        body {
            font-family: Arial, sans-serif;
            padding: 20px;
            line-height: 1.6;
        }

        h1 {
            color: #333;
        }

        .toc {
            padding: 10px;
            background-color: #f9f9f9;
            margin-bottom: 20px;
            border: 1px solid #ddd;
            border-radius: 5px;
            font-size: 16px;
        }

        .toc ul {
            list-style-type: none;
            padding-left: 0;
        }

        .toc li {
            margin-bottom: 10px;
        }

        .toc a {
            text-decoration: none;
            color: #0077cc;
        }

        .toc a:hover {
            text-decoration: underline;
        }

        .content-section {
            margin-bottom: 30px;
        }

        .content-section h2 {
            color: #4CAF50;
        }

        .content-section h3 {
            color: #2196F3;
        }

        .content-section p {
            margin: 15px 0;
        }

    </style>
</head>
<body>

    <h1>文章标题</h1>

    <!-- 目录 -->
    <div class="toc">
        <h3>目录</h3>
        <ul id="toc-list">
            <!-- 目录项会在这里通过 JavaScript 自动生成 -->
        </ul>
    </div>

    <!-- 月建冲爻指的是，卦中之爻与起卦当月月建相冲的情况，又称为月破

> 1.1 月建冲爻
    月建冲爻的时限性，一般来说，只在月内发挥作用，如测月内事逢月破则衰败。若为长远之事，则出月后不一定不吉。
    月建冲爻分为五类,月冲静爻、月冲动爻、月冲变爻、月冲飞神、月冲伏神。
    月建冲爻的两个重要信息
第一个是：月建代表过去。一般被月建冲破的爻，必定会应验出过去或当月出现了什么破败的事情的迹象。
二：月建代表当月。预示着卦中出现的破败现象发生在当月。 -->
    <div class="content">
        <div id="section-1" class="content-section">
            <h2>第一小节：介绍月建</h2>
            <p>这是文章的第一小节，内容介绍了文章的背景、目的以及大致结构。</p>
        </div>

        <div id="section-2" class="content-section">
            <h2>第二小节：深入分析</h2>
            <h3>子小节 1：数据分析</h3>
            <p>这里是第二小节的内容，介绍了数据分析方法与结果。</p>

            <h3>子小节 2：图表展示</h3>
            <p>在这一部分，我们展示了相关图表，帮助解释数据。</p>
        </div>

        <div id="section-3" class="content-section">
            <h2>第三小节：结论与未来展望</h2>
            <p>这是文章的结论部分，分析了研究结果并提出未来的展望。</p>
        </div>
    </div>

    <!-- 目录生成脚本 -->
    <script>
        // 获取所有的标题（h2 和 h3 标签）
        const headings = document.querySelectorAll('h2, h3');
        
        // 生成目录的列表项
        const tocList = document.getElementById('toc-list');

        headings.forEach((heading, index) => {
            // 为每个标题生成一个唯一的 id（如果没有 id，给它加上）
            if (!heading.id) {
                heading.id = 'section-' + (index + 1);
            }

            // 创建目录链接
            const tocItem = document.createElement('li');
            const tocLink = document.createElement('a');
            tocLink.href = `#${heading.id}`;
            tocLink.textContent = heading.textContent;

            // 为 h2 和 h3 使用不同的缩进
            if (heading.tagName === 'H2') {
                tocItem.style.marginLeft = '0px';
            } else if (heading.tagName === 'H3') {
                tocItem.style.marginLeft = '20px';
            }

            tocItem.appendChild(tocLink);
            tocList.appendChild(tocItem);
        });
    </script>

</body>
</html>


    


