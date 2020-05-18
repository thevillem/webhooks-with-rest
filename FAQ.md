# Webhooks + REST FAQ - test

## Where can I find the presentation slides?

You can download it from [here](https://speakerdeck.com/bswinnerton/building-github-integrations-with-webhooks-and-rest).

## What do I need to get started?

The workshop code and pre reqs can be found [here](https://github.com/githubsatelliteworkshops/webhooks-with-rest#mega-prerequisites).

## What do I need to do to clean up?

Inside the workshop's code root folder, run the following script:

```bash
script/reset
```

It should kill both the webserver and ngrok.

## I just want to see the complete code. What do I do?

To see everything running, you still need to setup everything mentioned in the [workshop guide](https://github.com/githubsatelliteworkshops/webhooks-with-rest/blob/master/workshop.md ).

But if you just want to see the full code, run the following in your terminal:

```bash
git clone git@github.com:githubsatelliteworkshops/webhooks-with-rest.git

cd webhooks-with-rest

git checkout verify-webhooks
```

Majority of the code lives under `webhooks-with-rest/changelogger/app/controllers/webhooks_controller.rb`

## What's the difference between GitHub Actions vs Webhooks?

GitHub Actions is built on top of GitHub Apps and webhooks and is tuned towards helping you with your CI/CD needs.

Outside of that domain, you can use webhooks to trigger other automations such as when other users interact with your repo.

## Where can I manage my GitHub Webhooks? And how do I redeliver a webhook?

You can add, edit, and delete your webhooks [here](https://github.com/jovel/webhooks-with-rest/settings/hooks).

When you edit a webhook, you can scroll all the way to the bottom to the section called `Recent Deliveries`. Click on ellipsis to the right of each webhook to expand the content. There should be a `Redeliver` button.

## How do I create a personal access token (PAT)?

Create a new personal access token [here](https://github.com/settings/tokens/new).

More detailed instructions can be found in our [help docs](https://help.github.com/en/github/authenticating-to-github/creating-a-personal-access-token-for-the-command-line).

## I'm getting 404 when I navigate to GitHub Pages. What do I do?

Sorry, you'll have to wait for a little bit. It takes Pages a few minutes to build before it can display the content.
