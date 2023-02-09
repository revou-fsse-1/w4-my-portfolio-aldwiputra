# Deployment and Custom Domain Setup

In this explanation, I'll show the process of deploying a project to Netlify and setting up a custom domain acquired from a local Domain Registrar 🌐, connect it to Cloudfare and finally Netlify.

<br/>

## :rocket: Deployment

### 1. Sign up to Netlify

If you don't have an account yet, you can sign up through a few options provided by Netlify.
![netlify-signup](/assets/sign-up-netlify.png)

### 2. Connect a Project

- Choose the Git provider where your site's source code is hosted.
  ![connect-project](/assets/connect-project.png)
- Pick a repository to connect
  ![pick-repository](/assets/pick-repository.png)
- Deploy site. Voilà! Your website is up. Everytime you make changes to the repository, the website will be automatically rebuilt and redeployed.
  ![deploy-netlify](/assets/deploy-netlify.png)

<br/>

## :globe_with_meridians: Custom Domain Setup

### 1. Buy domain through Domain Registrar

Choose a domain registrar that's most convenient for you.

### 2. Connect the domain you just bought to Cloudfare

- Sign up first if you aren't registered yet. Then go to **Dashboard** and click the button `+ Add Site`. Put your custom domain name in.
  ![add-site](/assets/add-site-cloudfare.png)
- After adding site, the nameservers listed on the Domain Registrar must be replaced with the ones provided by Cloudflare.
  Go to your Domain Registrar and replace them with the ones from Cloudflare.
  ![nameservers](/assets/nameservers.png)
  ![nameservers-niaga](/assets/nameservers-niaga.png)
- The process of changing nameservers could take up to 24 hours. So you need to wait before you domain is active on Cloudfare.
  ![24-hours](/assets/24-hours.png)

### 3. Add CNAME record

After your domain is active on Cloudfare, you need to add CNAME Record and point it to your Netlify subdomain.
![add-cname](/assets/add-cname.png)

### 4. Add custom domain to Netlify

After the domain setup is finished, it's finally time to add it to Netlify, so your website can be accessed from the custom domain address! 🎊

- Go to Netlify Dashboard and navigate to the project you want your custom domain to be pointed to. And within `Setup Site` section and choose `Set up a custom domain`.
  ![netlify-custom-domain](/assets/netlify-custom-domain.png)
- Put your custom domain in.
  ![custom-domain](/assets/put-in-custom-domain.png)
- All finished! You might need to wait before the site can be actually accessed.
  ![domain](/assets/domain.png)

---

Yeay my Personal Website is now live on **[https://aldwiputra.site](https://aldwiputra.site)**. Kindly check it out, and I hope you'll give me feedback on what could be improved ✌🏼.
![aldwiputra-site](/assets/aldwiputra-site.png)
