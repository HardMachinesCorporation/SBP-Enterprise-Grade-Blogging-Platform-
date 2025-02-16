Here’s a structured user flow diagram in text format based on the SBP platform’s core features:  

```
[Start]
   │
   ├──► [Landing Page]
   │        ├── About / Info (Optional)
   │        ├── Sign Up (Registration) ──► [Successful Registration] ──► [Dashboard]
   │        ├── Login ──► [Successful Login] ──► [Dashboard]
   │        ├── Forgot Password ──► [Password Reset] ──► [Login]
   │
   ├──► [Dashboard]
   │        ├── Blog Feed ──► View Posts
   │        │                  ├──► Edit Post
   │        │                  ├──► Delete Post (Confirmation)
   │        │                  ├──► Comment on Post (Optional)
   │        │
   │        ├── Create New Post ──► Publish Post ──► [Blog Feed]
   │        │
   │        ├── My Posts ──► Edit / Delete Post
   │        │
   │        ├── Profile ──► View / Edit Profile
   │        │
   │        ├── Settings ──► Privacy / Notification Settings
   │        │
   │        ├── Notifications (Optional) ──► View Updates
   │        │
   │        ├── Logout ──► [Landing Page]
   │
[End]
```
