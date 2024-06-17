# ad_buying_agent
AI Agent for Ad Media Buying

Basic Version - v1
----

1. User Input:
```
Create a detailed strategy and campaign based on the information provided.
Here are the inputs for the ad campaign:
budget: 200
duration: 7
target_audience: Females aged 18-45, interested in pottery, handmade crafts, home decor, and sustainable living, located in urban areas of the United States.
campaign_objectives: ["Increase brand awareness", "Boost engagement", "Generate inquiries for custom designs"]
```

2. Generated Strategy and Campaign:
```
{
  "budget": 200,
  "duration": 7,
  "target_audience": {
    "location": "Urban areas of the United States",
    "age": "18-45",
    "gender": "Female",
    "interests": ["Pottery", "Handmade crafts", "Home decor", "Sustainable living"],
    "behaviors": ["Online shopping", "Engagement with similar brands", "Interest in custom designs"]
  },
  "campaign_objectives": ["Increase brand awareness", "Boost engagement", "Generate inquiries for custom designs"],
  "ad_formats": ["Image Ads", "Video Ads", "Carousel Ads"],
  "best_times_days": {
    "days": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
    "times": ["7-9 AM", "6-9 PM"]
  },
  "ad_copy": {
    "image_ads": [
      "Discover the beauty of handmade pottery. Unique designs crafted with love. 🌿 #SustainableLiving #HandmadeCrafts",
      "Transform your home with our exclusive handmade decor. Custom designs available! 🏡 #HomeDecor #PotteryLove"
    ],
    "video_ads": [
      "Watch the magic of pottery come to life. Custom designs just for you! ✨ #Craftsmanship #PotteryArt",
      "From our hands to your home. Experience the art of handmade pottery. 🎨 #HandmadeWithLove #SustainableLiving"
    ],
    "carousel_ads": [
      "Swipe to explore our collection of handmade pottery. Perfect for your home! 🏠 #HandmadeCrafts #HomeDecor",
      "See the journey of our pottery from clay to masterpiece. Custom designs available! 🌟 #PotteryProcess #UniqueDesigns"
    ]
  },
  "visual_guidelines": {
    "resolution": "High",
    "highlight": "Craftsmanship and uniqueness",
    "lifestyle_shots": "Include",
    "branding": "Consistent with logo and brand colors"
  },
  "content_calendar": {
    "day_1": "Image Ad - Discover the beauty of handmade pottery.",
    "day_2": "Video Ad - Watch the magic of pottery come to life.",
    "day_3": "Carousel Ad - Swipe to explore our collection of handmade pottery.",
    "day_4": "Image Ad - Transform your home with our exclusive handmade decor.",
    "day_5": "Video Ad - From our hands to your home.",
    "day_6": "Carousel Ad - See the journey of our pottery from clay to masterpiece.",
    "day_7": "Image Ad - Discover the beauty of handmade pottery."
  },
  "campaign_structure": {
    "ad_sets": ["Image Ads", "Video Ads", "Carousel Ads"],
    "individual_ads": "As per content calendar"
  },
  "budget_allocation": {
    "total_budget": 200,
    "daily_budget": 28.57,
    "allocation": "Evenly across ad sets"
  }
}
```

3. Synthetic Report Data from Instagram API for the above Campaign:
```
report= """ Instagram Ad Campaign Report
Overall Campaign Metrics
Total Impressions: 250,000
Total Reach: 150,000
Total Engagement: 35,000
Likes: 25,000
Comments: 5,000
Shares: 3,000
Saves: 2,000
Click-through Rate (CTR): 1.8%
Total Clicks: 4,500
Conversion Rate: 0.5%
Total Conversions: 225
Inquiries for Custom Designs: 100
Newsletter Signups: 125
Cost Per Click (CPC): $0.44
Cost Per Thousand Impressions (CPM): $0.80
Total Spend: $200
Ad Set Specific Metrics
Image Ads:

Impressions: 100,000
Reach: 65,000
Engagement: 14,000
Likes: 10,000
Comments: 2,000
Shares: 1,200
Saves: 800
Clicks: 1,800
Conversions: 90
Spend: $50
CTR: 1.8%
CPC: $0.28
Video Ads:

Impressions: 80,000
Reach: 50,000
Engagement: 12,000
Likes: 8,000
Comments: 2,500
Shares: 1,000
Saves: 500
Clicks: 1,600
Conversions: 70
Spend: $75
CTR: 2%
CPC: $0.47
Carousel Ads:

Impressions: 70,000
Reach: 35,000
Engagement: 9,000
Likes: 7,000
Comments: 500
Shares: 800
Saves: 700
Clicks: 1,100
Conversions: 65
Spend: $75
CTR: 1.57%
CPC: $0.68
Key Insights
Highest Engagement: Video ads showed the highest engagement and click-through rate, highlighting the effectiveness of video content in capturing the attention of the target audience.
Cost Efficiency: Image ads provided the most cost-effective results in terms of cost per click and engagement.
Audience Interaction: Carousel ads generated significant interaction, especially in terms of shares and saves, indicating high interest in browsing multiple products.
Recommendations for Future Campaigns
Increase Budget on Video Ads: Given the high engagement and CTR, allocating a larger portion of the budget to video ads could maximize overall campaign effectiveness.
Experiment with Ad Timing: Analyzing the performance of ads at different times of the day could further optimize reach and engagement.
Enhance Carousel Ads: Focus on improving the call-to-action in carousel ads to increase clicks and conversions.

"""
```

4. New Strategy and Campaign Setting based on the report:
```
{
  "budget": 200,
  "duration": 7,
  "target_audience": {
    "location": "Urban areas of the United States",
    "age": "18-45",
    "gender": "Female",
    "interests": ["Pottery", "Handmade crafts", "Home decor", "Sustainable living"],
    "behaviors": ["Online shopping", "Engagement with similar brands", "Interest in custom designs"]
  },
  "campaign_objectives": ["Increase brand awareness", "Boost engagement", "Generate inquiries for custom designs"],
  "ad_formats": ["Video Ads", "Image Ads", "Carousel Ads"],
  "best_times_days": {
    "days": ["Monday", "Tuesday", "Wednesday", "Thursday", "Friday"],
    "times": ["7-9 AM", "12-2 PM", "6-9 PM"]
  },
  "ad_copy": {
    "image_ads": [
      "Discover the beauty of handmade pottery. Unique designs crafted with love. 🌿 #SustainableLiving #HandmadeCrafts",
      "Transform your home with our exclusive handmade decor. Custom designs available! 🏡 #HomeDecor #PotteryLove"
    ],
    "video_ads": [
      "Watch the magic of pottery come to life. Custom designs just for you! ✨ #Craftsmanship #PotteryArt",
      "From our hands to your home. Experience the art of handmade pottery. 🎨 #HandmadeWithLove #SustainableLiving"
    ],
    "carousel_ads": [
      "Swipe to explore our collection of handmade pottery. Perfect for your home! 🏠 #HandmadeCrafts #HomeDecor",
      "See the journey of our pottery from clay to masterpiece. Custom designs available! 🌟 #PotteryProcess #UniqueDesigns"
    ]
  },
  "visual_guidelines": {
    "resolution": "High",
    "highlight": "Craftsmanship and uniqueness",
    "lifestyle_shots": "Include",
    "branding": "Consistent with logo and brand colors"
  },
  "content_calendar": {
    "day_1": "Video Ad - Watch the magic of pottery come to life.",
    "day_2": "Image Ad - Discover the beauty of handmade pottery.",
    "day_3": "Carousel Ad - Swipe to explore our collection of handmade pottery.",
    "day_4": "Video Ad - From our hands to your home.",
    "day_5": "Image Ad - Transform your home with our exclusive handmade decor.",
    "day_6": "Carousel Ad - See the journey of our pottery from clay to masterpiece.",
    "day_7": "Video Ad - Watch the magic of pottery come to life."
  },
  "campaign_structure": {
    "ad_sets": ["Video Ads", "Image Ads", "Carousel Ads"],
    "individual_ads": "As per content calendar"
  },
  "budget_allocation": {
    "total_budget": 200,
    "allocation": {
      "video_ads": 100,
      "image_ads": 60,
      "carousel_ads": 40
    }
  }
}
```

Further Improvements
-----
- Better prompting techniques
- Use LangChain's LangGraph to create an AI Agentic flow with human-in-the-loop
