## AWS S3 Glacier – The best option for your backups?

It's been a while since I started to write on technical topics, here we go. Most of you who have many documents, photos and precious files in your phone or computer need a backup solution. I thought of letting you know –  AWS (Amazon Web Services) offers various tiers in their S3 (Simple Storage Service) service. Also, AWS S3 can be used for all cloud file hosting needs. Before we dive deep into the benefits, let us ask ourselves some questions.

**Is device storage not enough?**

For sure is – until you feel you need a backup. Even if you have a phone or a computer with reasonably ample storage, you will often need a safe place to store your files apart from the hardware in your hand. The device might get bricked or lost; you don't have control over these acts. So, a place to store your files safely should always be a top concern for you.

**Free storage services, Dropbox and Google Photos?**

Great question. Everything you get for free has a hidden price, i.e. your privacy. As long as the data you hold is not sensitive and is not an issue for you if it went to the wrong hands, it's okay to share the data with the services mentioned above. Even with those, there's always a hard limit on the maximum capacity for a specific account. For example, Google limits to 15 GB, Apple with 5 GB, Dropbox usually under 2GB, and Google Photos limits unlimited free storage uploads for compressed low-quality photos.
Dropbox, Mega, and their competitors do reasonably well – not an issue with their privacy at all. This article is to detail the advantages and disadvantages of S3 tiers alone, don't get offended. Also, does Dropbox allow you to store more than 3TB at the end of the day?


> The caveat here is that many people have terabytes of data and still struggle to find a perfect solution. People like hardcore photographers (like me) with tons of RAW images, those handling sensitive documents, codebases, etc., still need solutions.

**S3 tiers and their pricing**

AWS S3 offers various product tiers; each catered carefully for the type of data and frequency you will store and access. The common ones used are Standard, Intelligent, Glacier, and Deep Glacier.

***Standard***

If you want daily backup files and access them frequently, I don't recommend S3 since the cost you spend could be more. For this type of ask, the Standard tier is the best way to store. It costs $0.025 per GB flat without any other charges. Note that the costs mentioned in this article are for a month. So, if you store 1 TB data in this tier, it will likely cost you $20 per month – still a sweet deal, but the data management will not be easy as in Dropbox or iCloud.

***Glacier / Deep Glacier***

Just inversely proportional to the Standard tier. These tiers are the best for people who want to store their files somewhere safe and will not access them at all. Lifelong storage of photos, your works, etc., can be some examples. I use this service to backup all the RAW images I take from my camera.

The storage costs are as follows,

Glacier - $0.005 per GB

Deep Glacier - $0.002 per GB

So, it will only cost you $5 per month and $2 per month for Glacier and Deep Glacier respectively for storing 1 TB of data.

What's the difference between Glacier and Deep Glacier, you might ask. Unlike the Standard tier, Glacier tiers have additional costs associated with them. Along with the storage costs, you need to pay specific fees each time you download the files back from S3.

The retrieval fees are as follows,

Glacier - $0.012 per GB
Deep Glacier - $0.024 per GB

So, it will cost you $12 and $24 for Glacier and Deep Glacier respectively for retrieving 1 TB  data back to your computer from S3.

This is obvious since AWS offers you low prices, which you won't get from other cloud storage providers. Moreover, you are not expected to frequently access these files and only on a need basis you will probably try to access them, i.e. rarely. So, the costs are saving for you in the long term.

***Intelligent***

This tier is for those who don't know their data storage volume and the frequency of access in the short term. AWS has launched this tier so that you can save costs automatically. When you access your files frequently, it changes your files to the Standard tier in the back to incur no retrieval costs. In contrast, if you don't access the files for a certain time, the storage costs are lowered, and retrieval costs are increased – it moves to the Glacier tiers we discussed above. Usually not recommended unless you are double sure – people do have their preferences, primarily for backups.

For more details on the pricing, check out AWS S3 pricing directly - https://aws.amazon.com/s3/pricing/.

Thanks for reading, I hope you got some cloud insights. PT.