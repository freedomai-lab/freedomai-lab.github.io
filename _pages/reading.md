---
layout: page
permalink: /playground/
title: Playground
description:
years: [2025, 2026]
nav: true
nav_order: 2
---

<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <style>
        .ai-model-showcase * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        .ai-model-showcase-body {
            font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
            background: #ffffff;
            min-height: 100vh;
            padding: 20px;
        }

        .ai-model-showcase-container {
            max-width: 1200px;
            margin: 0 auto;
        }

        .ai-model-showcase-page-title {
            text-align: center;
            color: #2d3748;
            font-size: 2rem;
            font-weight: 700;
            margin-bottom: 2rem;
        }

        .ai-model-showcase-cards-grid {
            display: flex;
            flex-direction: column;
            gap: 1.5rem;
            max-width: 800px;
            margin: 0 auto;
        }

        .ai-model-showcase-card {
            background: white;
            border-radius: 12px;
            box-shadow: 0 4px 12px rgba(0, 0, 0, 0.1);
            padding: 16px;
            display: flex;
            align-items: flex-start;
            gap: 16px;
            transition: all 0.3s ease;
            position: relative;
            overflow: hidden;
            border: 1px solid #e2e8f0;
        }

        .ai-model-showcase-card::before {
            content: '';
            position: absolute;
            top: 0;
            left: 0;
            right: 0;
            height: 4px;
            background: linear-gradient(90deg, #667eea, #764ba2);
        }

        .ai-model-showcase-card:hover {
            transform: translateY(-2px);
            box-shadow: 0 8px 20px rgba(0, 0, 0, 0.15);
        }

        .ai-model-showcase-avatar {
            width: 60px;
            height: 60px;
            border-radius: 8px;
            object-fit: cover;
            border: 2px solid #f0f0f0;
            flex-shrink: 0;
        }

        .ai-model-showcase-card-content {
            flex: 1;
            min-width: 0;
        }

        .ai-model-showcase-model-name {
            font-size: 1.25rem;
            font-weight: 700;
            color: #2d3748;
            margin-bottom: 8px;
            line-height: 1.3;
        }

        .ai-model-showcase-model-description {
            color: #4a5568;
            line-height: 1.5;
            margin-bottom: 12px;
            font-size: 0.9rem;
        }

        .ai-model-showcase-links-container {
            display: flex;
            flex-wrap: wrap;
            gap: 8px;
        }

        .ai-model-showcase-badge {
            display: inline-flex;
            align-items: center;
            gap: 6px;
            padding: 6px 12px;
            background-color: #e2e8f0;
            color: #4a5568;
            text-decoration: none;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 500;
            transition: all 0.2s ease;
            border: 1px solid transparent;
        }

        .ai-model-showcase-badge:hover {
            background-color: #cbd5e0;
            color: #2d3748;
            transform: translateY(-1px);
            box-shadow: 0 2px 8px rgba(0,0,0,0.1);
        }

        .ai-model-showcase-badge.ai-model-showcase-demo {
            background-color: #e6fffa;
            color: #234e52;
            border-color: #81e6d9;
        }

        .ai-model-showcase-badge.ai-model-showcase-demo:hover {
            background-color: #b2f5ea;
        }

        .ai-model-showcase-badge.ai-model-showcase-github {
            background-color: #f7fafc;
            color: #2d3748;
            border-color: #e2e8f0;
        }

        .ai-model-showcase-badge.ai-model-showcase-github:hover {
            background-color: #edf2f7;
        }

        .ai-model-showcase-badge.ai-model-showcase-huggingface {
            background-color: #fef5e7;
            color: #744210;
            border-color: #f6e05e;
        }

        .ai-model-showcase-badge.ai-model-showcase-huggingface:hover {
            background-color: #faf089;
        }

        .ai-model-showcase-icon {
            width: 16px;
            height: 16px;
        }

        .ai-model-showcase-open-source-badge {
            position: absolute;
            top: 12px;
            left: 12px;
            background: linear-gradient(135deg, #48bb78, #38a169);
            color: white;
            padding: 4px 8px;
            border-radius: 6px;
            font-size: 0.75rem;
            font-weight: 600;
            box-shadow: 0 2px 4px rgba(72, 187, 120, 0.3);
            z-index: 10;
        }

        @media (max-width: 768px) {
            .ai-model-showcase-card {
                flex-direction: column;
                text-align: center;
            }

            .ai-model-showcase-avatar {
                align-self: center;
            }
        }
    </style>
</head>
<body class="ai-model-showcase-body">
    <div class="ai-model-showcase-container">

        <div class="ai-model-showcase-cards-grid">
            <!-- 模型卡片 1 -->
            <div class="ai-model-showcase-card">
                <img src="https://cdn-1.webcatalog.io/catalog/discord-bot-list/discord-bot-list-icon-filled-256.png?v=1714774149420" alt="GPT-4 Avatar" class="ai-model-showcase-avatar">
                <div class="ai-model-showcase-card-content">
                    <h2 class="ai-model-showcase-model-name">Image Generation: Janus-4o</h2>
                    <p class="ai-model-showcase-model-description">
                        Janus-4o is a multimodal model that can generate high-quality images from text or from text and images, trained on just 91K samples made by GPT-4o.
                    </p>
                    <div class="ai-model-showcase-links-container">
                        <a href="#" class="ai-model-showcase-badge ai-model-showcase-demo">
                            <svg class="ai-model-showcase-icon" viewBox="0 0 24 24" fill="currentColor">
                                <path d="M12 2L2 7v10c0 5.55 3.84 9.95 9 11 5.16-1.05 9-5.45 9-11V7l-10-5z"/>
                            </svg>
                            在线体验
                        </a>
                        <a href="#" class="ai-model-showcase-badge ai-model-showcase-github">
                            <svg class="ai-model-showcase-icon" viewBox="0 0 24 24" fill="currentColor">
                                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                            </svg>
                            GitHub
                        </a>
                        <a href="#" class="ai-model-showcase-badge ai-model-showcase-huggingface">
                            <svg class="ai-model-showcase-icon" viewBox="0 0 24 24" fill="currentColor">
                                <path d="M12 2.5c-5.25 0-9.5 4.25-9.5 9.5s4.25 9.5 9.5 9.5 9.5-4.25 9.5-9.5-4.25-9.5-9.5-9.5zm0 17c-4.14 0-7.5-3.36-7.5-7.5s3.36-7.5 7.5-7.5 7.5 3.36 7.5 7.5-3.36 7.5-7.5 7.5z"/>
                            </svg>
                            Hugging Face
                        </a>
                    </div>
                </div>
            </div>

            <!-- 模型卡片 2 -->
            <div class="ai-model-showcase-card">
                <div class="ai-model-showcase-open-source-badge">开源</div>
                <img src="https://cdn-1.webcatalog.io/catalog/discord-bot-list/discord-bot-list-icon-filled-256.png?v=1714774149420" alt="Claude Avatar" class="ai-model-showcase-avatar">
                <div class="ai-model-showcase-card-content">
                    <h2 class="ai-model-showcase-model-name">Medical LLM: HuatuoGPT-II</h2>
                    <p class="ai-model-showcase-model-description">
                        HuatuoGPT-II uses a unified input-output format for domain adaptation and achieves top performance in Medical, even surpassing GPT-4 in some tasks.
                    </p>
                    <div class="ai-model-showcase-links-container">
                        <a href="https://www.huatuogpt.cn/" class="ai-model-showcase-badge ai-model-showcase-demo">
                            <svg class="ai-model-showcase-icon" viewBox="0 0 24 24" fill="currentColor">
                                <path d="M12 2L2 7v10c0 5.55 3.84 9.95 9 11 5.16-1.05 9-5.45 9-11V7l-10-5z"/>
                            </svg>
                            在线体验
                        </a>
                        <a href="#" class="ai-model-showcase-badge ai-model-showcase-github">
                            <svg class="ai-model-showcase-icon" viewBox="0 0 24 24" fill="currentColor">
                                <path d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.30.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z"/>
                            </svg>
                            GitHub
                        </a>
                        <a href="#" class="ai-model-showcase-badge ai-model-showcase-huggingface">
                            <svg class="ai-model-showcase-icon" viewBox="0 0 24 24" fill="currentColor">
                                <path d="M12 2.5c-5.25 0-9.5 4.25-9.5 9.5s4.25 9.5 9.5 9.5 9.5-4.25 9.5-9.5-4.25-9.5-9.5-9.5zm0 17c-4.14 0-7.5-3.36-7.5-7.5s3.36-7.5 7.5-7.5 7.5 3.36 7.5 7.5-3.36 7.5-7.5 7.5z"/>
                            </svg>
                            Hugging Face
                        </a>
                    </div>
                </div>
            </div>

        </div>
    </div>
</body>
</html>
