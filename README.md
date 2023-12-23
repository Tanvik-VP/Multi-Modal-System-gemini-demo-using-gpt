# Building Gemini demo using GPT vision

This project will utilize the GPT-4 Vision API to achieve our objectives.

The following technical requirements are essential for this experiment:

The process needs to be executed in real-time.
Users should have the capability to stream video.
Interaction with the assistant should be possible through voice commands, eliminating the need for UI interaction.
The assistant is required to interpret and analyze the video input to address the user's queries.
The assistant's responses should be delivered audibly.

## Steps:
1. Make sure you install all npm dependencies
2. Download this repository and run " npm start dev " in your terminal.
3. Add your OPENAI API key in the below window and also add in language which you want to use, OPENAI uses many language transcripts
<img width="1622" alt="Screenshot 2023-12-22 at 7 23 39 PM" src="https://github.com/Tanvik-VP/gemini-demo-using-gpt/assets/77459265/add8d0e0-166f-43af-a23d-81565cbddff7">


## How this project works:
First we use the image and get the past maximum screenshots and create an image grid and store it in online tmp storage and return the url back to the model.
for voice we send the recording to whisper and get it back as the prompt and again send it to the GPT 4V model
![Blank diagram](https://github.com/Tanvik-VP/gemini-demo-using-gpt/assets/77459265/d690b6b2-7b8e-43de-8b43-94b9f8aa44b8)


## Results:


https://github.com/Tanvik-VP/gemini-demo-using-gpt/assets/77459265/ce504066-2536-4737-9198-2ac0cc91bd3d


Input: What am I holding in my hand?
<img width="1120" alt="Screenshot 2023-12-22 at 7 39 59 PM" src="https://github.com/Tanvik-VP/gemini-demo-using-gpt/assets/77459265/7d101d71-98dc-4008-85fb-4d5477a85d6b">

Input: Which is the best book to learn about advance Machine Learning?
<img width="847" alt="Screenshot 2023-12-22 at 7 42 38 PM" src="https://github.com/Tanvik-VP/gemini-demo-using-gpt/assets/77459265/69c237db-92da-4282-8367-43bcc45216a6">

<img width="901" alt="Screenshot 2023-12-22 at 7 41 57 PM" src="https://github.com/Tanvik-VP/gemini-demo-using-gpt/assets/77459265/28e79ec4-d5d5-4b4a-877d-f35912fc9098">

Although the latency of response is too bad, it takes around 5-10 sec to respond, but the responses are good.

you can try it out.

## References:
This is the complex version of this project and Jidé did a really good job on building this.
https://www.crafters.ai/aitools/rebuild-gemini-demo-with-gpt-4-vision

<br>
<br>


### Default instructions:
<br>
This is a [Next.js](https://nextjs.org/) project bootstrapped with [`create-next-app`](https://github.com/vercel/next.js/tree/canary/packages/create-next-app).

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.
Check out AI JASON in youtube.
Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.


