
ѵ��������
1. ��SCIR_triplet_net.prototxt����SCIR_pairwise_net.prototxt���ĵ�10��source��Ϊ���ݼ�ͼ��ĸ�Ŀ¼����11��image_files��Ϊѵ��ͼ����б��ļ�
2. ��SCIR_triplet_solver.prototxt����SCIR_pairwise_solver.prototxt���ĵ�17��loss_file��Ϊ��¼ÿ�ε�����ʧ����ֵ���ļ�������18�и�Ϊ��¼ѵ�������м�������������ļ���ǰ׺
3. ����SCIR_triplet_train.sh����SCIR_pairwise_train.sh��

���Է�����
1. ���ȶ�probe set��gallery set����lmdb
2. SCIR_triplet_test_solver.prototxt����SCIR_pairwise_test_solver.prototxt���ĵ�2�и�Ϊprobe image����
3. SCIR_triplet_test_net.prototxt�ĵ�32�и�Ϊprobe set��lmdbλ�ã���48�и�Ϊgallery set��lmdbλ�ã���50�и�Ϊgallery image����
4. SCIR_triplet_test.sh����SCIR_pairwise_test.sh����5�и�Ϊ���������snapshot�ļ�
5. ����SCIR_triplet_test.sh����SCIR_pairwise_test.sh��
6. �����Ժ���configĿ¼�»�����cost3.txt��cost4.txt��pairwiseģ����lossSI.txt��cost4.txt����cost3.txt����lossSI.txt����single-image representation��distance matrix��cost4.txt��cross-image representation��loss matrix
7. ��matlab������testmatching(SIRfile,CIRfile,probelabel,gallerylabel,setting)�õ�matching accuracy��SIRfile��cost3.txt����lossSI.txt����·����CIRfile��cost4.txt��·����probelabel��gallerylabel�ֱ���probe image��gallery image��label��setting��'singleshot'����'multishot'