����̏I���ɗ~���s�����ƃI�i������A�䖝���ĕ����Ă��炢�ɗ��邯��
�Z�t���Ȃ�I�i�j�[�������Ă��炢�ɂ���ė����������炵���񂶂�Ȃ������Ă��Ƃō쐬�B

[���e]
����̏I���̃I�i�j�[�^�C���ɂ�
���Ȃ��Ƃ̊֌W���ɂ���Ď��Ԃ��䖝���āA���Ȃ��̏Z��ł���Ƃ���ɖK�₷��m�����オ��܂��B

���~ > ���� > �Z�t���A���l > �v�� �̏��Ŋm��UP


�ꉞ����m�Fver : eraTW4.571


[�X�V����]
2018/01/08	�K���Ɋ���


[�����t�@�C���ύX�_�������p����]
AFTERTRA.ERB
404�s	ELSEIF CFLAG:LOCAL:���܂��Ă�x > ���Ԕ���臒l
�̉���
		LOCAL:1 = 0
		IF TALENT:LOCAL:���~
			LOCAL:1 = 5
		ELSEIF TALENT:LOCAL:����
			LOCAL:1 = 4
		ELSEIF TALENT:LOCAL:�Z�t��
			;���l������
			LOCAL:1 = 3
		ELSEIF TALENT:LOCAL:�v��
			LOCAL:1 = 2
		ENDIF
		IF TALENT:LOCAL:�����S && LOCAL:1 < 5
			LOCAL:1 += 1
		ENDIF
		IF CFLAG:LOCAL:�������� & ����_���ӂ� && !RAND:(7 - LOCAL:1)
��ǉ�
