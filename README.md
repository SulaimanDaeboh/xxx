กดที่ +แล้วกดที่ repository

cd Desktop
git clone [URL]
git clone https://github.com/SulaimanDaeboh/xxx		ตัวอย่าง
cd xxx							เข้าไปที่โฟล์เดอร์ xxx ที่ clone 
git init
git add . 						ใส่ไปทั้งหมด
git status 						แสดงสถานะ
git commit -m "first commit"
git config --global user.email "man.sd.9@gmail.com"
git config --global user.name "SulaimanDaeboh"
git remote add origin https://github.com/SulaimanDaeboh/xxx.git
git push -u origin master

git commit -m "xxx"
git log --oneline
git reset --soft "HEAD^"				ลบที่ commit 
git reset HEAD .					ลบไฟล์

git add .
git commit -m "me"
git push

git checkout -b Miew					สร้าง Branches ชื่อ Miew แล้วไปหามันเลย
git add .
git commit -m "miew"
git push --set-upstream origin Miew

git checkout master 					เปลี่ยนไปอยู่ที่ Branches -> master
git merge Miew						รวม Branches อื่นๆมาเป็นอันเดียว
git push						ใส่ที่มัดลงในเว็บ
git merge --no-ff Miew

git log --oneline
git checkout cd46f5a					cd46f5a คือที่เราจะย้อนไป
git checkout master					ย้อนกลับปัจจุบัน

git branch -d Miew					ลบ branch ของ Miew 
git push origin --delete Miew				ลบ remote branch ของ Miew ที่ต่อกับเว็บ 

git tag vl.25						สร้าง tag
git tag vl.26
git push origin --tags
git tag --delete vl.25					ลบ tag
git push origin --delete vl.25				ลบ remote ของ tag นั้นที่ต่อกับเว็บ
