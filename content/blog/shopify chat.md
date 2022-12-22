---

description: Initial description.

author: "@Luigi"
---

## Shopify Support
- Hi, we need to customize our site's Checkout page, we want to be able to do modifications that the regular settings -> checkout -> customize checkout doesn't have. 
  The checkout template code isn't in our codebase as well.
  
  Please let me know how to proceed. We would like to do this changes in our test environment (dztesting.myshopify.com) and also in our production store ([https://spotonfence.com/](https://spotonfence.com/))
  
  Here are the Store owner details:
  NAME
  Karen Polcaro
  EMAIL
  [karen@spotonfence.com](mailto:karen@spotonfence.com)
  PHONE
  [karen@spotonfence.com](mailto:karen@spotonfence.com)
  
  Thanks a lot.
- Chat started with Raziel
- Raziel
  
  Thanks for reaching out to Shopify! Raziel here, your Advisor for today.
  
  Hi Luis! I have read your message above and thank you so much for the information! I will be assisting you today and we'll get through this together.
  
  Can you provide me a screenshot on how you wanted to customize your check out page so that I can take a closer look?
- Sure
  
  #+BEGIN_EXPORT hiccup
  [:a {:target "_blank", :rel "noopener noreferrer", :href "https://storage.googleapis.com/chat-attachments-production/2022-12-07/beba2204-67f6-4d31-9582-97830a5ac716/Y3VzdG9tIGNoZWNrb3V0ICgxKS5wbmc="} [:img {:src "https://storage.googleapis.com/chat-attachments-production/2022-12-07/beba2204-67f6-4d31-9582-97830a5ac716/Y3VzdG9tIGNoZWNrb3V0ICgxKS5wbmc=", :alt ""}]]
  #+END_EXPORT
  
  For instance we want to put the html code on the bottom right
  
  Where it says "Why choose...." and display some icons and text there in a similar way as in the screenshot
- Raziel
  
  Thank you for the screenshot, Luis! I just wanna confirm, this is the current check out page for the store and your team wanted to add the screenshot from the bottom right at this part. 
  #+BEGIN_EXPORT hiccup
  [:a {:onmouseout "this.style['text-decoration'] = 'underline'; this.style['color'] = '#2c6ecb'", :onmouseover "this.style['text-decoration'] = 'underline'; this.style['color'] = '#1f5199'", :href "https://shopify.click/81573-34557-19903-98528-51109.png", :target "_blank", :rel "noopener noreferrer"} [:img {:alt "", :src "https://shopify.click/81573-34557-19903-98528-51109.png"}]]
  #+END_EXPORT
  
  Am I correct?
- Correct, totally
  
  In case it helps, here is the current checkout page:
  
  #+BEGIN_EXPORT hiccup
  [:a {:target "_blank", :rel "noopener noreferrer", :href "https://storage.googleapis.com/chat-attachments-production/2022-12-07/bf813984-fea5-4695-98e6-9d5c45fd8712/Y2hlY2tvdXQgc2FtcGxlIGN1cnJlbnQucG5n"} [:img {:src "https://storage.googleapis.com/chat-attachments-production/2022-12-07/bf813984-fea5-4695-98e6-9d5c45fd8712/Y2hlY2tvdXQgc2FtcGxlIGN1cnJlbnQucG5n", :alt ""}]]
  #+END_EXPORT
- Raziel
  
  I appreciate it! I have to check this one with our resources. One moment please!
- No problem
- Raziel
  
  Thank you so much for patiently waiting! As for this, we can edit the checkout page. By selecting Themes > Customize theme > Checkout, you can access several options for personalizing the Checkout within the Theme Editor. Beyond that, nothing can be manually altered. The reason for this is because the source code is not made public since the Checkout page is secured. This makes it easier to guarantee the security of both the merchant's and the customers' information at all times.
  
  Your request is indeed possible however, I'm afraid customization of this magnitude would fall outside of the scope of design support we can provide. I am fully aware how important this is to you but we would highly suggest hiring a Shopify Expert. An additional workaround for this would be posting a job in our [Shopify Experts Site](https://experts.shopify.com/) if this can be done via a coding mechanism. The good news is that posting a job on our Expert Site will be free, with no charge at all. Charges will only prevail if you and the expert will have an agreement.
- I'm a developer myself, I could do it in my own if I was able to access the checkout template code.
  
  I've been told I can contact support (this is what I am doing right now) and I could get the checkout template's code to be able to change it. 
  I understand the security reasons and that is why I provided the Store owner contact details from the beginning.
  Please can you confirm or not if my assumption is right? And how to proceed in order to be able to do the job?
- Raziel
  
  Let me verify that one here, hold on Luis!
  
  Thank you for keeping the chat open.
  
  Still checking this with our support team.
  
  I appreciate your patience here.
  
  I would like to ask Luis, if you have already checked it here as well?
  
  One moment let me send a screenshot.
  
  As per checking, the check out liquid can only be unlocked for Shopify Plus 
   merchants. Here is a helpful document I found about [https://shopify.dev/themes/architecture/layouts/checkout-liquid](https://shopify.dev/themes/architecture/layouts/checkout-liquid)
  
  As per checking, the check out liquid can only be unlocked for Shopify Plus
  merchants. Here is a helpful document I found about [Checkout liquid](https://shopify.dev/themes/architecture/layouts/checkout-liquid).
- Yes we are already Shopify Plus merchants, that's the reason why I came here to ask for access checkout.liquid
- Raziel
  
  Thank you Luis for keeping the chat always open. I really understand how important this is but the main reason why it's not letting us access the checkout template code is because this is only for the Shopify