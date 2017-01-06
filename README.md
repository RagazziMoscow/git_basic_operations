# ������� �������� � Git
��� ����������� ��������� �������� ��������, ������� ����� ����� ������ � �����.  
����� ���������� ����� ������������ � �������� � ���������� ������ �� �������, ������ �������� ������� ��� �������� ���� ���� Git-book'a.  
 
#������
### ��������� ����� ���������
����, �� ������ �� ������. ��� � ��������� ������ ��������� ���� �������� �� ���������,  
������� ������� ������� �����?  

��� ������ � ��������� ������������� ���������� [fetch, merge � pull](https://git-scm.com/book/ru/v1/������-Git-������-�-���������-�������������):  
`$ git fetch server_branch` \# ������ ������ �� ������ �����  
`$ git merge server_branch` \# ����� ������ ����� � ������� �������  

���  

`$ git pull server_branch master` \#  ��� �������� ����� ��������  

������� �� ������� `$ git merge` ������ ������� ����� ��������� [������� ����� Git-book'a](https://git-scm.com/book/ru/v2/%D0%92%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D0%B2-Git-%D0%9E-%D0%B2%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B8-%D0%B2-%D0%B4%D0%B2%D1%83%D1%85-%D1%81%D0%BB%D0%BE%D0%B2%D0%B0%D1%85).    

--------------------------------------------------
###���������� ������ ����������� � ���������
�� ���, �� ���������. ������ ����� ���������� ����� ����� � �������. ���?  

���������� [git push](https://git-scm.com/book/ru/v1/%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D1%8B-Git-%D0%A0%D0%B0%D0%B1%D0%BE%D1%82%D0%B0-%D1%81-%D1%83%D0%B4%D0%B0%D0%BB%D1%91%D0%BD%D0%BD%D1%8B%D0%BC%D0%B8-%D1%80%D0%B5%D0%BF%D0%BE%D0%B7%D0%B8%D1%82%D0%BE%D1%80%D0%B8%D1%8F%D0%BC%D0%B8#Push):  
`$ git push origin master`  

����� ����� ��������, ������ �� ���������� ������ [push � ������](https://developer.atlassian.com/blog/2015/04/force-with-lease/).  

--------------------------------------------------
### ����������� � �����������
��� ������� ��������� ���� ��������� �� ������ �� �����, ��� ���� ������� ������� ��� �� ����, ��� � ��, ������ ���������, ����� ������ ����������. ��� ����?   

����� ���������� ������� ����� ����� ���������� ������ � ������� ������� ���������� ������� `$ git diff`.  
� ���, ��� �� ������������ ����� �������� �� [���������������](http://stackoverflow.com/questions/3338126/how-to-diff-the-same-file-between-two-different-commits-on-the-same-branch).  
� ���� ��������� ��� ��� ���������: ���� ��� �������, �� ��� �������� ��� �������� � ���.  

� PyCharm ����� ��������� ������ �������� ������� � ��������� ��� � �������. [������ �� ������������](https://www.jetbrains.com/help/pycharm/2016.1/using-
-integration.html)   

--------------------------------------------------
### ����������� �����
������ ��� ���� ������. ���������� �� �������� ������ "����� � ����������". ����� �� �������, ��� ��� ������, �� ��������� ���-�� ��� �������. ��� ������-��?  

`$ git branch feature_branch`  # �������� ����� �����  
`$ git checkout feature_branch` # ������� � ����� �����  

���  

`$ git checkout -b feature_branch` # ��� �������� ����� ��������  

����������� ����������� ����� ��� ��������� ������������� ����� ����� �� � ��� �� [Git-book](https://git-scm.com/book/ru/v2/%D0%92%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D0%B2-Git-%D0%9E-%D0%B2%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B8-%D0%B2-%D0%B4%D0%B2%D1%83%D1%85-%D1%81%D0%BB%D0%BE%D0%B2%D0%B0%D1%85).  

--------------------------------------------------
### ����� ���� ���������
������ �� ��������, ������ �� ������� �������� "���������� ���� ����� � ���". ��� ��� �� ����? ��� ������?  

�� �� �� ������ ����� � ���, ������ ����, �������� �������:   
`$ git checkout dev_branch` # ������������� �� ����� dev  
`$ git merge work_branch` # ������� ����� work_branch  

--------------------------------------------------
### �������� � ���� ����� ��������� �� ������
��������� ������ �� ������� ��� ��, � ��������� ����� �� ����. ������, �����: ��� ������ ������, � ������ �� ������. ��� ��� �������� "������� ��������� �� ���� � ���� �����". ���?  

`$ git merge dev` # ��������� ������� ������� ����� dev � my_branch, �������� � ����� my_branch   
`$ git checkout dev` # ��������� � ����� dev  
`$ git merge my_branch` # ������ ��� ������� dev � my_branch  

--------------------------------------------------
### ��������� ������
�� ������ ������, �� ������ � ������, � ������� ���������: ������ ���� ������ ������ � ������. ������, ��� �� �������. ������ ���� ���� ������ ��������� � ���. ��� ��� �������?  

���������� [git cherry-pick](https://git-scm.com/docs/git-cherry-pick) � [git reset](https://git-scm.com/book/ru/v2/%D0%98%D0%BD%D1%81%D1%82%D1%80%D1%83%D0%BC%D0%B5%D0%BD%D1%82%D1%8B-Git-%D0%A0%D0%B0%D1%81%D0%BA%D1%80%D1%8B%D1%82%D0%B8%D0%B5-%D1%82%D0%B0%D0%B9%D0%BD-reset):  
`$ git cherry-pick 62ecb3` # �������� �������, �������� � ����� dev. ������ ������� ������ �� ������� ��������� ����� � ������ ����� ��������, � ����� ������ �� dev � master. `62ecb3` - ��� ���������� �������  
`$ git �ommit -m "Commit message`  # ������� ������ ��� � ����� �����  
`$ git checkout master` # ��������� � master  
`$ git reset --hard HEAD` # �������� ���������� ������� ������ � ���������������� �������  

--------------------------------------------------
### �������� ������
��������� ��� ������� � ����� ����� �, �����, ���������, ��� ������ ������ ��� ��� ��� ������� �����... ��� ����������?

�����������, ��� ��� ��������� �������:  
`$ git commit -m "Change header style with a mistake"`  
`$ git commit -m "Change header style with a crytical mistake"`  

��� ���� ��������� � ��������� ����������� �� ������ ������, ��� ��� ��� ����� ������. ����� ���� ����� ������ ���������, ������ ��� ��������� ����������� "C" (�� ����� correct).  

������ ������:     
`$ git reset HEAD~2` # ���������� ������ �������� � ��� ��������������� ����� ������ `unstaged`, � ��������� ����������� ������ "C".   
�������� ���� ������ � ����, ������ ��� ��������� �������;
`$ git add index.html`  
`$ git commit -m 'Change header style`  

����� ����� ������������ `git commit -c ORIG_HEAD`, ����� �� ������ �� �� ����� ��������� ������� ������.  

������ ������:  
`$ git commit revert HEAD~2` # �� ���� �����, �� ����������: ������� ������ ����� ������ c ���������� ����������� "C", �� ������ ���������� ������� � �� ������ ��������� �����. 

��������� � ������ �������� � �������� �������������� ���������� ����� �������� [�����](https://githowto.com/ru/undoing_committed_changes).   

--------------------------------------------------
### ������� �������, ������� ���� �������� �� �������� ������
��� �� ��� ������ ������� ���� �������� � ���������� "��������� ������ 3" �� ����� �� github?  

���������� [git rebase](https://git-scm.com/book/ru/v1/%D0%92%D0%B5%D1%82%D0%B2%D0%BB%D0%B5%D0%BD%D0%B8%D0%B5-%D0%B2-Git-%D0%9F%D0%B5%D1%80%D0%B5%D0%BC%D0%B5%D1%89%D0%B5%D0%BD%D0%B8%D0%B5):  
`$ git rebase -i origin/master~4 master`  
`$ git push origin +master`   

��� �� [���������������](http://stackoverflow.com/questions/8981194/changing-git-commit-message-after-push-given-that-no-one-pulled-from-remote) ����������� ��� push � ������.  

--------------------------------------------------
### �������� ������� � ��������� ������ ��� ������������� ���  
�������� �����, �� ����� ��������� �������...  

���������� [git commit --amend](https://git-scm.com/book/ru/v1/%D0%9E%D1%81%D0%BD%D0%BE%D0%B2%D1%8B-Git-%D0%9E%D1%82%D0%BC%D0%B5%D0%BD%D0%B0-%D0%B8%D0%B7%D0%BC%D0%B5%D0%BD%D0%B5%D0%BD%D0%B8%D0%B9):  
`$ git commit -m "Add description"` # ������� ������   
`$ git add README.md` # ��������� ��� �������, ��������������� � �������� ������ ����   
`$ git commit --amend` # ������� ������� ��������� � ��������� ������ c ������������ ������������� ��� ���������   

����� ������ ������������� ���������� ������, ����� ������������ �� �� ������ ������, ������ �� �������� � �� ������� ����� �����������:  
`$ git commit -m "Add description"`  
`$ git commit --amend`  

--------------------------------------------------
� �� �������� ��� �������� ��������� c����� �� ���������� - ["���������� Git"](https://habrahabr.ru/post/28268/).  

# Contributing

����� ������? ������ ��������������? ���� ��� � slack @beastrock ��� [���������](http://vk.com/beastrock).
