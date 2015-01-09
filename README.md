#git-svn实战

#svn checkout
echo 9OWM56vKeaoUEmex | git svn clone --no-auth-cache --username rsync svn://192.168.0.1/trunk trunk

cd ask
git branch aaa      #临时分支
git checkout aaa    #切换分支
touch test.txt      #编辑
git add .           #添加
git commit -m 'aaa' #提交
git checkout master #切回master
git merge aaa       #合并分支
git branch -d aaa   #删除分支

#svn update
echo 9OWM56vKeaoUEmex | git svn rebase --no-auth-cache --username rsync

#svn commit
echo 9OWM56vKeaoUEmex | git svn dcommit --no-auth-cache --username rsync
