# Easy Instagram Automation Service MCP Server

English | [简体中文](./README.md) | [繁體中文](./README_ZH-TW.md)

## 🚀 Quick Start with EMCP Platform

**[EMCP](https://sit-emcp.kaleido.guru)** is a powerful MCP server management platform that allows you to quickly use various MCP servers without manual configuration!

### Quick Start:

1. 🌐 Visit **[EMCP Platform](https://sit-emcp.kaleido.guru)**
2. 📝 Register and login
3. 🎯 Go to **MCP Marketplace** to browse all available MCP servers
4. 🔍 Search or find this server (`bach-easy_instagram_automation_service`)
5. 🎉 Click the **"Install MCP"** button
6. ✅ Done! You can now use it in your applications

### EMCP Platform Advantages:

- ✨ **Zero Configuration**: No need to manually edit config files
- 🎨 **Visual Management**: Easy-to-use GUI for managing all MCP servers
- 🔐 **Secure & Reliable**: Centralized API key and authentication management
- 🚀 **One-Click Install**: Rich selection of servers in MCP Marketplace
- 📊 **Usage Statistics**: Real-time service call monitoring

Visit **[EMCP Platform](https://sit-emcp.kaleido.guru)** now to start your MCP journey!


---

## Introduction

This is an MCP server for accessing the Easy Instagram Automation Service API.

- **PyPI Package**: `bach-easy_instagram_automation_service`
- **Version**: 1.0.0
- **Transport Protocol**: stdio


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

## Configuration

### API Authentication

This API requires authentication. Please set environment variable:

```bash
export API_KEY="your_api_key_here"
```

### Environment Variables

| Variable | Description | Required |
|----------|-------------|----------|
| `API_KEY` | API Key | Yes |




### 在 Claude Desktop 中使用

编辑 Claude Desktop 配置文件 `claude_desktop_config.json`:


```json
{
  "mcpServers": {
    "easy_instagram_automation_service": {
      "command": "uvx",
      "args": ["--from", "bach-easy_instagram_automation_service", "bach_easy_instagram_automation_service"],
      "env": {
        "API_KEY": "your_api_key_here"
      }
    }
  }
}
```

**Note**: Replace `E:\path\to\easy_instagram_automation_service\server.py` with the actual server file path.


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

This server is automatically generated by [API-to-MCP](https://github.com/BACH-AI-Tools/api-to-mcp) tool.

Version: 1.0.0
