�Ƽ����ְ��ֽ���ʹ��Git http://blog.jobbole.com/78960/

�ڱ� git �����Ŀ¼��ɾ���ļ�ʱ������ѡ���������ַ�ʽ����¼ɾ��������
һ��rm + git commit -am "abc"
����git rm + git commit -m "abc"
���⣬git add . ���ܼ�¼��ӡ��Ķ��Ķ�����ɾ���Ķ����迿 git rm ����ɡ�
���rm ɾ�����ļ��Ǵ��� not staged ״̬�ģ�
Ҳ����һ�ֽ��� ��δ�Ķ��� �� �����ύ���� ֮���״̬��


git checkout . #���������޸ĵġ�û�е��ύ�ģ������ص�ԭ����״̬
git stash #������û���ύ���޸��ݴ浽stash���档����git stash pop�ظ���
git reset --hard HASH #���ص�ĳ���ڵ㣬�������޸ġ�
git reset --soft HASH #���ص�ĳ���ڵ㡣�����޸�


һ�� git clean�������git reset ʹ�õ� 
������е��޸��Լ������ݴ����Ļ� 
��ô 
git reset --hard 
git clean -xdf 
���û�м����ݴ����Ļ� git checkout . && git clean -xdf


git checkout -f //checkout���ļ����е��ļ�