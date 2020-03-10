# test for open redirect vulnerabilities (passively) 


| dork | injection param |
|:---:|:---:|
| inurl:redirect= | - |
| inurl:rdir=  | - |
| inurl:to=  | FP |
| inurl:destination= | - |
| inurl:ReturnURL=  | - |
| inurl:redirect_uri= | - |
| inurl:/allowcookies= | - |
| inurl:next= | - |
| inurl:url=https | - |
| inurl:url=http | - |
| inurl:redirect?https | - |
| inurl:redirect?http | - |
| inurl:url=http | - |
| inurl:link=http| - |
| inurl:link=https| - |

# TIP 
* do search excluding words that can include fp and links that include login because often will require login to redirect
use something like: 

Example: 

inurl:logout?returnUrl= -checkout -tickets -user -docs -kr  -account  -signup -signin -login -support -enroll -register -questions -logon -help -signin -log -password
