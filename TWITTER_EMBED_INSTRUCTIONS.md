# Twitter/X Embed Instructions

## How to Add Your Actual Tweets

### Step 1: Get Your Tweet URLs
1. Go to your Twitter/X profile: https://twitter.com/prashanthvarma
2. Find the tweets you want to embed
3. Click on the tweet to open it
4. Copy the URL from the address bar

### Step 2: Extract Tweet ID
From a tweet URL like: `https://twitter.com/prashanthvarma/status/1234567890123456789`
The tweet ID is: `1234567890123456789`

### Step 3: Update the HTML
In `_includes/twitter.html`, replace the placeholder URLs:

```html
<!-- Replace YOUR_TWEET_ID_1 with actual tweet ID -->
<blockquote class="twitter-tweet" data-theme="light" data-dnt="true" data-lang="en">
    <a href="https://twitter.com/prashanthvarma/status/ACTUAL_TWEET_ID_1"></a>
</blockquote>
```

### Step 4: Example with Real Tweet
If you want to embed a tweet with ID `1234567890123456789`:

```html
<blockquote class="twitter-tweet" data-theme="light" data-dnt="true" data-lang="en">
    <a href="https://twitter.com/prashanthvarma/status/1234567890123456789"></a>
</blockquote>
```

## Tweet Embed Options

### Available Parameters:
- `data-theme="light"` - Light theme (or "dark")
- `data-dnt="true"` - Do Not Track (privacy)
- `data-lang="en"` - Language
- `data-cards="hidden"` - Hide tweet cards
- `data-conversation="none"` - Hide conversation

### Example with All Options:
```html
<blockquote class="twitter-tweet" 
    data-theme="light" 
    data-dnt="true" 
    data-lang="en"
    data-cards="hidden"
    data-conversation="none">
    <a href="https://twitter.com/prashanthvarma/status/YOUR_TWEET_ID"></a>
</blockquote>
```

## Recommended Tweets to Embed

1. **Professional achievements** - New role, project launches
2. **Technical insights** - Industry thoughts, technology trends
3. **Conference talks** - Speaking engagements, presentations
4. **Company updates** - Graphiant news, team highlights
5. **Personal milestones** - Awards, recognitions

## Troubleshooting

### Tweet Not Loading?
1. Check if the tweet ID is correct
2. Ensure the tweet is public
3. Verify the Twitter widget script is loaded
4. Check browser console for errors

### Styling Issues?
1. The CSS is already optimized for embedded tweets
2. Tweets will automatically resize to fit the container
3. Mobile responsiveness is handled automatically

## Best Practices

1. **Keep it fresh** - Update tweets regularly
2. **Mix content** - Professional and personal tweets
3. **Engage** - Include tweets that show interaction
4. **Quality over quantity** - Choose meaningful tweets
5. **Test regularly** - Ensure embeds work after updates
