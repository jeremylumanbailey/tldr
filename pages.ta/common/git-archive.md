# git archive

> பெயரிடப்பட்ட மரத்திலிருந்து கோப்புகளின் காப்பகத்தை உருவாக்கவும்.
> மேலும் தகவல்: <https://git-scm.com/docs/git-archive>.

- தற்போதைய HEAD இன் உள்ளடக்கங்களிலிருந்து ஒரு தார் காப்பகத்தை உருவாக்கி அதை நிலையான வெளியீட்டில் அச்சிடுக:

`git archive --verbose HEAD`

- தற்போதைய HEAD இலிருந்து ஒரு ஜிப் காப்பகத்தை உருவாக்கி அதை நிலையான வெளியீட்டில் அச்சிடுக:

`git archive --verbose --format=zip HEAD`

- மேலே உள்ளதைப் போலவே, ஆனால் கோப்புக்கு ஜிப் காப்பகத்தை எழுதவும்:

`git archive --verbose --output={{கோப்புக்கான/பாதை/கோப்பு.zip}} HEAD`

- ஒரு குறிப்பிட்ட கிளையில் சமீபத்திய உறுதிப்பாட்டின் உள்ளடக்கங்களிலிருந்து தார் காப்பகத்தை உருவாக்கவும்:

`git archive --output={{கோப்புக்கான/பாதை/கோப்பு.tar}} {{கிளை_பெயர்}}`

- ஒரு குறிப்பிட்ட கோப்பகத்தின் உள்ளடக்கங்களிலிருந்து தார் காப்பகத்தை உருவாக்கவும்:

`git archive --output={{கோப்புக்கான/பாதை/கோப்பு.tar}} HEAD:{{கோப்பகத்திற்கான/பாதை}}`

- ஒவ்வொரு கோப்பிற்கும் ஒரு குறிப்பிட்ட கோப்பகத்திற்குள் காப்பகப்படுத்த ஒரு பாதையைத் தயாரிக்கவும்:

`git archive --output={{கோப்புக்கான/பாதை/கோப்பு.tar}} --prefix={{தயார்படுத்தும்/பாதை}}/ HEAD`