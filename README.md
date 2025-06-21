JSON Data Comparison AppThis web app helps you quickly compare two JSON lists: "Followers Data" and "Following Data". It shows you who's in one list but not the other, based on their "value" field.FeaturesLoad JSON: Easily import JSON data by pasting text or uploading .json files (up to 1MB each).Two-Way Difference: See items unique to your Followers list and items unique to your Following list.Condensed View: Results are displayed in a compact, readable grid to show more items at once.Smart Comparison: Ignores case differences for accurate matches.Clear Messages: Get instant feedback on loading and comparison status.How to UseOpen index.html in your browser.Load "Followers Data": Paste your JSON or upload its file.Load "Following Data": Paste your JSON or upload its file (this app handles the relationships_following structure).Click "Compare Lists".View the "Comparison Results" to see the differences.Expected JSON FormatsThe app focuses on the "value" field within the "string_list_data" array.Followers Data Example:[
  {
    "title": "User Profiles",
    "string_list_data": [
      { "value": "user_one" },
      { "value": "user_two" }
    ]
  }
]
Following Data Example:{
  "relationships_following": [
    {
      "title": "",
      "string_list_data": [
        { "value": "tanya_gijy" },
        { "value": "user_three" }
      ]
    }
  ]
}
Technical DetailsBuilt with HTML, CSS (Tailwind CSS), and JavaScript.All processing happens in your browser; no data is sent to a server.LimitationsEach JSON file must be under 1MB.Comparison is strictly by the value field in string_list_data.