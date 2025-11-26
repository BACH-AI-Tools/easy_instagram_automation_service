# Easy Instagram Automation Service MCP Server

[English](./README_EN.md) | [简体中文](./README.md) | 繁體中文

## 🚀 使用 EMCP 平台快速體驗

**[EMCP](https://sit-emcp.kaleido.guru)** 是一個強大的 MCP 伺服器管理平台，讓您無需手動配置即可快速使用各種 MCP 伺服器！

### 快速開始：

1. 🌐 造訪 **[EMCP 平台](https://sit-emcp.kaleido.guru)**
2. 📝 註冊並登入帳號
3. 🎯 進入 **MCP 廣場**，瀏覽所有可用的 MCP 伺服器
4. 🔍 搜尋或找到本伺服器（`bach-easy_instagram_automation_service`）
5. 🎉 點擊 **「安裝 MCP」** 按鈕
6. ✅ 完成！即可在您的應用中使用

### EMCP 平台優勢：

- ✨ **零配置**：無需手動編輯配置檔案
- 🎨 **視覺化管理**：圖形介面輕鬆管理所有 MCP 伺服器
- 🔐 **安全可靠**：統一管理 API 金鑰和認證資訊
- 🚀 **一鍵安裝**：MCP 廣場提供豐富的伺服器選擇
- 📊 **使用統計**：即時查看服務調用情況

立即造訪 **[EMCP 平台](https://sit-emcp.kaleido.guru)** 開始您的 MCP 之旅！


---

## 簡介

這是一個使用 [FastMCP](https://fastmcp.wiki) 自動生成的 MCP 伺服器，用於存取 Easy Instagram Automation Service API。

- **PyPI 套件名**: `bach-easy_instagram_automation_service`
- **版本**: 1.0.0
- **傳輸協定**: stdio


## 安装

### 从 PyPI 安装:

```bash
pip install bach-easy_instagram_automation_service
```

### 从源码安装:

```bash
pip install -e .
```

## 运行

### 方式 1: 使用 uvx（推荐，无需安装）

```bash
# 运行（uvx 会自动安装并运行）
uvx --from bach-easy_instagram_automation_service bach_easy_instagram_automation_service

# 或指定版本
uvx --from bach-easy_instagram_automation_service@latest bach_easy_instagram_automation_service
```

### 方式 2: 直接运行（开发模式）

```bash
python server.py
```

### 方式 3: 安装后作为命令运行

```bash
# 安装
pip install bach-easy_instagram_automation_service

# 运行（命令名使用下划线）
bach_easy_instagram_automation_service
```

## 配置

### API 認證

此 API 需要認證。請設定環境變數:

```bash
export API_KEY="your_api_key_here"
```

### 環境變數

| 變數名 | 說明 | 必需 |
|--------|------|------|
| `API_KEY` | API 金鑰 | 是 |




### 在 Claude Desktop 中使用

编辑 Claude Desktop 配置文件 `claude_desktop_config.json`:


```json
{
  "mcpServers": {
    "easy_instagram_automation_service": {
      "command": "python",
      "args": ["E:\path\to\easy_instagram_automation_service\server.py"],
      "env": {
        "API_KEY": "your_api_key_here"
      }
    }
  }
}
```

**注意**: 請將 `E:\path\to\easy_instagram_automation_service\server.py` 替換為實際的伺服器檔案路徑。


## 可用工具

此服务器提供以下工具:


### `auth_login`

This endpoint will return back all information for use of instagram automation - Auth login

**端点**: `POST /auth/auth_login_auth_login_post`



---


### `timeline_feed`

This endpoint will return back all information for use of instagram automation - timeline feed

**端点**: `GET /auth/timeline_feed_auth_timeline_feed_get`



---


### `media_insights`

This endpoint will return back all information for use of instagram automation - Get insights data for media

**端点**: `POST /insights/media_insights_media_post`



---


### `account_insights`

This endpoint will return back all information for use of instagram automation - Get insights for account

**端点**: `POST /insights/account_insights_account_post`



---


### `media_feed_all`

This endpoint will return back all information for use of instagram automation - Return media with insights

**端点**: `POST /insights/media_feed_all_insights_media_feed_all_post`



---


### `story_from_url`

This endpoint will return back all information for use of instagram automation - Get Story (media) PK from URL

**端点**: `GET /story/story_pk_from_url_story_pk_from_url_get`



---


### `igtv_upload_by_url_copy`

This endpoint will return back all information for use of instagram automation - Upload photo by URL and configure to feed

**端点**: `POST /igtv/igtv_upload_igtv_upload_by_url_post`



---


### `igtv_download_by_url`

This endpoint will return back all information for use of instagram automation - Download IGTV video using URL

**端点**: `POST /igtv/igtv_download_by_url_igtv_download_by_url_post`



---


### `user_remove_follower`

This endpoint will return back all information for use of instagram automation - Remove a follower

**端点**: `POST /user/user_remove_follower_user_remove_follower_post`



---


### `username_from_user_id`

This endpoint will return back all information for use of instagram automation - Get username from user id

**端点**: `POST /user/username_from_user_id_user_username_from_id_post`



---


### `user_id_from_username`

This endpoint will return back all information for use of instagram automation - Get user id from username

**端点**: `POST /user/user_id_from_username_user_id_from_username_post`



---


### `user_unfollow`

This endpoint will return back all information for use of instagram automation - Unfollow a user

**端点**: `POST /user/user_unfollow_user_unfollow_post`



---


### `user_follow`

This endpoint will return back all information for use of instagram automation - Follow a user

**端点**: `POST /user/user_follow_user_follow_post`



---


### `user_info_by_username`

This endpoint will return back all information for use of instagram automation - Get user object from username

**端点**: `POST /user/user_info_by_username_user_info_by_username_post`



---


### `user_info`

This endpoint will return back all information for use of instagram automation - Get user object from user id

**端点**: `POST /user/user_info_user_info_post`



---


### `user_following`

This endpoint will return back all information for use of instagram automation - Get user's followers information

**端点**: `POST /user/user_following_user_following_post`



---


### `user_followers`

This endpoint will return back all information for use of instagram automation - Get user's followers

**端点**: `POST /user/user_followers_user_followers_post`



---


### `photo_upload_by_url`

This endpoint will return back all information for use of instagram automation - photo upload by url

**端点**: `POST /photo/photo_upload_photo_upload_by_url_post`



---


### `photo_download_by_url`

This endpoint will return back all information for use of instagram automation - photo download by url

**端点**: `POST /photo/photo_download_by_url_photo_download_by_url_post`



---


### `photo_upload_to_story_by_url`

This endpoint will return back all information for use of instagram automation - photo upload to story by url

**端点**: `POST /photo/photo_upload_to_story_by_url_photo_upload_to_story_by_url_post`



---


### `video_upload_by_url`

This endpoint will return back all information for use of instagram automation - video upload by url

**端点**: `POST /video/video_upload_video_upload_by_url_post`



---


### `video_download_by_url`

This endpoint will return back all information for use of instagram automation - video download by url

**端点**: `POST /video/video_download_by_url_video_download_by_url_post`



---


### `video_download`

This endpoint will return back all information for use of instagram automation - video download

**端点**: `POST /video/video_download_video_download_post`



---


### `video_upload_to_story_by_url`

This endpoint will return back all information for use of instagram automation - video upload to story by url

**端点**: `POST /video/video_upload_to_story_by_url_video_upload_to_story_by_url_post`



---


### `video_upload_to_story`

This endpoint will return back all information for use of instagram automation - video upload to story

**端点**: `POST /video/video_upload_to_story_video_upload_to_story_post`



---


### `media_likers`

This endpoint will return back all information for use of instagram automation - media likers

**端点**: `POST /media/media_likers_media_likers_post`



---


### `media_unlike`

This endpoint will return back all information for use of instagram automation - media unlike

**端点**: `POST /media/media_unlike_media_unlike_post`



---


### `like_media`

This endpoint will return back all information for use of instagram automation - like media

**端点**: `POST /media/media_like_media_like_post`



---


### `media_oembed`

This endpoint will return back all information for use of instagram automation - media oembed

**端点**: `POST /media/media_oembed_media_oembed_post`



---


### `user_media`

This endpoint will return back all information for use of instagram automation - user media

**端点**: `POST /media/user_medias_media_user_medias_post`



---


### `media_info`

This endpoint will return back all information for use of instagram automation - media info

**端点**: `POST /media/media_info_media_info_post`



---


### `auth_relogin`

This endpoint will return back all information for use of instagram automation - Auth relogin

**端点**: `POST /auth/auth_relogin_auth_relogin_post`



---



## 技术栈

- **FastMCP**: 快速、Pythonic 的 MCP 服务器框架
- **传输协议**: stdio
- **HTTP 客户端**: httpx

## 开发

此伺服器由 [API-to-MCP](https://github.com/BACH-AI-Tools/api-to-mcp) 工具自動生成。

版本: 1.0.0
