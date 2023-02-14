# React 4

## Dynamic Routes

- Dynamic Routes can be created by using square brackets in the page file name, e.g. [id].js.
- The value between the brackets will be available in the page component as a query parameter.
- The getStaticPaths function is used to specify which paths should be pre-rendered at build time.
- The getStaticProps function is used to fetch the data for a specific path at build time or at request time.
- Dynamic Routes can also be created using the useRouter hook in a functional component.
- Dynamic Routes are useful for creating pages that display unique content, such as product pages, user profiles, and blog post pages.

##  Deployment

- Vercel platform was developed by the creators of Next.js so it is the easiest way to deploy
- Vercel is a serverless platform used for both static/hybrid applications
- DPS stands for Develop, Preview and Ship and it is a helpful workflow to utilize
- Develop: Write your code in Next.js and use the development server to see how everything renders/looks
- Preview: Utilize the Vercel preview deployment
- Ship: Merge pull request back to main before shipping the code to production
- Next.js can be deployed to other hosting providers that also support Node.js, but Vercel is just the best option

### Things I want to know more about

- I'd like to know more about deploying and how it works with react.

### Sources

- <https://nextjs.org/learn/basics/dynamic-routes>
- <https://nextjs.org/learn/basics/deploying-nextjs-app>
- <https://www.youtube.com/watch?v=JWCS5IdECVI>
- <https://nextjs.org/docs/basic-features/static-file-serving>

[Back To Home](../README.md)