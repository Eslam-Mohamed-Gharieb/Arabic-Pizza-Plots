# Arabic-Pizza-Plots

## مقارنة لاعبي الدوريات الخمس الكبري [اسبانيا، إيطاليا، إنجلترا، فرنسا، والمانيا] بناءاً علي نسبهم المئوية وفقاً لشركة "ستاتس بومب" وموقع "سمارت سكاوت" الشهيرين 


#### النسب المئوية هي ترتيب كل لاعب مقارنة بأصحاب المركز في الدوريات الخمس الكبري في مدي يبدأ من 1 وينتهي ب 100.
كمثال: إذا كان ترتيب لاعب ما 5 في إحصائية الأهداف المتوقعه، هذا يعني أنه 95% من لاعبي المركز يمتلكون رقماً أعلي منه في هذه الإحصائية.


<p float="center">
<img src="https://user-images.githubusercontent.com/73742092/206175530-7744925e-d708-473c-92ea-8e6e1a802910.png" width="250"> 
<img src="https://user-images.githubusercontent.com/73742092/206175557-2796b5df-36e6-4c59-a9f4-4fe966f49918.png" width="250">
</p>


## خطوات إنتاج الصور من الـ Notebooks :
- فتح الـ Notebook أولا
- إدخل إسم اللاعب في هذا الموقع https://www.arabic-text.com/ ونسخ الإسم بالمقلوب (مشاكل تخص لغة البرمجة بايثون في التعامل مع اللغة العربية)
- وضع إسم اللاعب في المكان المخصص له player_name
- كتابة ثم نسخ إسم الفريق كذلك ووضعه في المكان المخصص له player_team
- الدخول علي https://fbref.com وكتابة إسم اللاعب الذي تريد عمل خريطة له ثم نقل عنوان الصفحة

 بعد الدخول علي صفحة اللاعب عليك إختيار الـ Scouting report المطلوب رسمه..
بالنسبة للاعب يلعب في الدوري الفرنسي، فالريبورت المطلوب لموسم 22/23 هو كما موضح بالصورة. ننقر عليه ثم وننسخ لينك اللاعب ونضعه في الـ Notebook في المكان المخصص له 
player_fbref_link

<img src="https://user-images.githubusercontent.com/73742092/206179893-3cb3f5a9-5fc6-425c-9bb6-fde42c467ddb.png" width="500">


الخطوة الأخيرة هي تغيير إسم الصورة التي سيتم حفظها، وهذا من خلال هذا الأمر 
plt.savefig('مبابي.png',facecolor=fig.get_facecolor(), dpi=300, bbox_inches='tight')

تغيير مبابي لأي إسم أخر تفضله ومن ثم حفظ الصورة علي جهازك.
