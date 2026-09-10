#dainik varta

Simple Hindi news website — static HTML, कोई backend नहीं चाहिए।

## Deploy on Vercel (GitHub के ज़रिए)

1. GitHub पर नया repository बनाओ (नाम कुछ भी रख सकते हो, जैसे `dainik varta`)
2. इस folder के सारे files (`index.html`) उस repo में upload/push करो
3. [vercel.com](https://vercel.com) पर जाओ → Sign up (GitHub से)
4. "Add New" → "Project" → अपनी repo select करो
5. Framework "Other" ही रहने दो, कुछ change मत करो
6. "Deploy" दबाओ — कुछ सेकंड में live link मिल जाएगा

## नया article कैसे जोड़ें

`index.html` खोलो, `const articles = [ ... ]` वाला हिस्सा ढूंढो। ऊपर एक नई entry जोड़ो इस format में:

```js
{
  id: 5,
  title: "यहां headline लिखो",
  excerpt: "यहां 1-2 लाइन का summary लिखो",
  img: "यहां image का URL डालो",
  date: "10 सितंबर 2026",
  body: [
    "पहला paragraph यहां",
    "दूसरा paragraph यहां"
  ]
}
```

Save करके GitHub पर push करते ही Vercel अपने आप site update कर देगा।
