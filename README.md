# schedule

打ち合わせ管理リポジトリ。Google Calendar 連携 + Slack 通知。

## 機能

| ワークフロー | 機能 |
|---|---|
| `add-meeting.yml` | 打ち合わせ → Google Calendar 登録（バッティングチェック付き） |
| `daily-schedule.yml` | 毎朝9:00 に今日の打ち合わせを Slack 通知 |
| `auto-label.yml` | Issue に「打ち合わせ」ラベルを自動付与 |
| `sync-calendar.yml` | Issue → Google Calendar 同期（作成/編集/Close対応） |

## 登録方法

1. **Google カレンダーから直接登録**
2. **Slack ワークフローから登録** → schedule リポに Issue 作成 → Calendar 自動同期
3. **GitHub Issue で確認・編集**

## 必要な Secrets

| Secret 名 | 用途 |
|---|---|
| `GOOGLE_SERVICE_ACCOUNT_KEY` | Google Calendar API 用サービスアカウント鍵 |
| `MEETING_CALENDAR_ID` | 打ち合わせ用カレンダーの ID |
| `SLACK_WEBHOOK_URL` | Slack 通知用 Webhook URL |

## 関連リポジトリ

- [work-tasks](https://github.com/toritoriri/work-tasks) — タスク管理（GTD + PARA）
