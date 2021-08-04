# Setup:

Create a Next.js app:

run the following command termeinal:

```
npx create-next-app nextjs-blog --use-npm --example "https://github.com/vercel/next-learn-starter/tree/master/learn-starter"

cd nextjs-blog

npm run dev
```

# Assets:

Next.js also has support for Image Optimization by default. This allows for resizing, optimizing, and serving images in modern formats like WebP when the browser supports it. This avoids shipping large images to devices with a smaller viewport. It also allows Next.js to automatically adopt future image formats and serve them to browsers that support those formats.

example:

```
import Image from 'next/image'

const YourComponent = () => (
  <Image
    src="/images/profile.jpg" // Route of the image file
    height={144} // Desired size with correct aspect ratio
    width={144} // Desired size with correct aspect ratio
    alt="Your Name"
  />
)

```

# Metadata :

we wanted to modify the metadata of the page, such as the `<title>` HTML tag

example:

Open the pages/posts/first-post.js file and add an import for Head from next/head at the beginning of the file:

```
import Head from 'next/head'

```

in component file :

```
export default function FirstPost() {
  return (
    <>
      <Head>
        <title>First Post</title>
      </Head>
      <h1>First Post</h1>
      <h2>
        <Link href="/">
          <a>Back to home</a>
        </Link>
      </h2>
    </>
  )
}

```
# Css:
Next.js has built-in support for CSS and Sass which allows you to import .css and .scss files.

Using popular CSS libraries like Tailwind CSS is also supported.

take a look at pages/index.js, you should see code like this:
```
<style jsx>{`
  …
`}</style>
```

for more info : [nextjs](https://nextjs.org/learn/basics/assets-metadata-css)