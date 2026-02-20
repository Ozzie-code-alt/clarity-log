# 🧠 Clarity Log

Clarity Log is a modern decision journal designed to help you track
important decisions, evaluate outcomes, and improve your judgment over
time.

Instead of forgetting why you made a decision, Clarity Log helps you
build a structured feedback loop for better thinking.

------------------------------------------------------------------------

## ✨ Why Clarity Log?

Most people:

-   Make decisions based on incomplete context\
-   Overestimate their confidence\
-   Repeat the same mistakes\
-   Forget lessons learned

Clarity Log helps you:

-   Log decisions with context\
-   Track expected vs actual outcomes\
-   Measure confidence accuracy\
-   Reflect on lessons learned\
-   Improve long-term judgment

------------------------------------------------------------------------

## 🚀 MVP Features

-   🔐 Authentication (Email + Password)
-   ➕ Create decisions
-   📋 View & filter decision history
-   🗓 Review decisions after review date
-   📊 Basic insights dashboard:
    -   Total decisions
    -   \% good vs bad outcomes
    -   Average confidence score
    -   Simple analytics overview

------------------------------------------------------------------------

## 🧱 Tech Stack

### Frontend

-   Next.js (App Router)
-   Tailwind CSS
-   TanStack Query
-   Zod (validation)

### Backend

-   Server Actions
-   PostgreSQL
-   Prisma ORM

### Authentication

-   Auth.js (Credentials Provider)

### Deployment

-   Vercel

------------------------------------------------------------------------

## 🗄 Database Schema (MVP)

### User

-   id
-   email
-   password_hash
-   created_at

### Decision

-   id
-   user_id
-   title
-   context
-   expected_outcome
-   confidence (1--10)
-   category
-   status ("open" \| "reviewed")
-   review_date
-   actual_outcome
-   result_rating ("good" \| "neutral" \| "bad")
-   lessons_learned
-   reviewed_at
-   created_at
-   updated_at

------------------------------------------------------------------------

## 📂 Project Structure

    app/
      dashboard/
      decision/
        new/
        [id]/
    lib/
      db/
      actions/
      auth/
    schema/
      decision.schema.ts
    components/

------------------------------------------------------------------------

## 🛠 Local Development

``` bash
# Install dependencies
npm install

# Setup database
npx prisma migrate dev

# Run development server
npm run dev
```

------------------------------------------------------------------------

## 🔐 Environment Variables

Create a `.env` file:

    DATABASE_URL=
    AUTH_SECRET=
    NEXTAUTH_URL=

------------------------------------------------------------------------

## 🎯 Roadmap

### Phase 1 (MVP)

-   Authentication
-   Decision CRUD
-   Review system
-   Insights dashboard

### Phase 2

-   Tags & filtering
-   Email reminders
-   Confidence analytics chart
-   Dark mode
-   Export to CSV

### Phase 3

-   AI pattern detection
-   Team decision tracking
-   Public reflection pages

------------------------------------------------------------------------

## 🧠 Core Philosophy

> Better decisions come from measured reflection.

Clarity Log is not just a note-taking app --- it is a system for
improving how you think.

------------------------------------------------------------------------

## 📄 License

MIT
