OrchartBS
=========

OrchartBS��֯�ܹ�ͼ�����������˵����

һ�������ʵ���˺�����������νṹ��֯�ܹ�ͼ��
������ʵ�����ӡ�ɾ�����ı�ڵ�ṹ�Ĺ��ܡ�
���������϶��ڵ㣬�ı�ڵ�ṹ��
�ġ�����������չ�ڵ���̬����ʽ��
�塢ͨ�������ֿ����ɷŴ���С��
�����϶��ڵ���Ҫȷ��document�ϵ�mouse�¼���Ч��

����ʵ����Դ�����е�chart.html������ʾ������chart-simple.html������ʾ����

���Ĵ��룺

window.CO = new CreateOrgchartBS($.extend({
	"data":data, //�ڵ�����	
	"wrap":$("#box_org_tree") //�ܹ�ͼ����
}, DemoOption));
window.CO.init();

�����ò�����
var defaultOption = {
	"wrap":this.conf.wrap,//jQuery���������ṹ����
	"orgType":this.conf.orgType,//�ַ������ṹ���ͣ�Ĭ��tree(����)����һ��column(��ʽ)
	"onStartMove":onStartMoveCallback,//�������϶���ʼǰִ�з����������������ƶ�������jQuery����
	"onEndMove":onEndMoveCallback,//�������϶�������ִ�з�����������{"node":[�����ƶ�������jQuery����],"oparent":[�����ƶ�������jQuery����ľɸ��ڵ�org_td]}
	"htmlContent":htmlContent,//�ַ��������ݣ��ڵ�����ģ��
	"createHtmlContent":createHtmlContent,//���������ݽڵ�����ģ��htmlContent����html�ڵ㣬������data��ǰ���ݽڵ�����{}
	"addEventToNode":addEventToNode,//��������html�ڵ�����¼���������item��ǰ���ݽڵ��jQuery����
	"onAppendNodeWithData":onAppendNodeWithData,//���������ѽڵ��һ�����ڵ��ƶ�����һ�����ڵ�󣬲�����{"node":[��ǰ�ƶ��ڵ�org_td],"oparent":[��ǰ�ƶ��ڵ�org_td�ľɸ��ڵ�org_td]}
	"onCancelOriginalPlaceholder":onCancelOriginalPlaceholder,//�������Ƴ��ƶ�ʱռλ(���߿�)���ִ�з��������������߿�jQuery����
	"onCreateGroupTreeCallback":onCreateGroupTreeCallback,//������������ͬ����ͬ��ڵ���ִ�з�������������ǰ��ĸ��ڵ����org_td,Ԫ���Ƿ�ִ��isExec
	"onCreateRankTreeCallback":onCreateRankTreeCallback,//������������ͬ���ڵ���ִ�з�����������i��ǰ�㼶��o��ǰ�㼶����,Ԫ���Ƿ�ִ��isExec
	"onCreateAllTreeCallback":onCreateAllTreeCallback,//������������ȫ���ڵ���ִ����������������֯�ṹ����������,Ԫ���Ƿ�ִ��isExec
	"onStartCreateAllTreeCallback":onStartCreateAllTreeCallback,//��������ʼ����ǰ��ִ�з�������������֯�ṹ����������
	"isMoveOperation":isMoveOperation,//�������Ƿ������϶��ڵ����������true or false��Ч
	"onDeleteNodeCallback":onDeleteNodeCallback
};