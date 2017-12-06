# C++�ɂ�����v�Z�ʂ̃I�[�_�[
* [mathjax enable]

���̋L���ł͎�ɁA�W�����C�u�����̃R���e�i�ƃA���S���Y���̌v�Z�ʂɂ��ĉ������B

## ��{�I�Ȍv�Z�ʂƁAC++�ɂ������\��

- �v�f���Ɉˑ����Ȃ��������F $O\left(1\right)$
- �v�f���Ɉˑ������������i�v�f�������炩�ȏꍇ�j: $O\left(n\right)$
- �v�f���Ɉˑ������������i�v�f�����v�Z����K�v������ꍇ�j: $O\left(\log n\right)$
- �\�[�g�𔺂�������: $O\left(n \log n\right)$

| �v�Z�ʁi���Ȃ����j | ���� | C++�ɂ������\�� |
|---|---|---|
| $O\left(1\right)$ | �萔����<br>(*constant*) | �f�t�H���g�R���X�g���N�^<br>�f�t�H���g�f�X�g���N�^<br>�f�X�g���N�^�i�q�v�f���������́j<br>���[�u�R���X�g���N�^<br>`swap` ����<br>���z��̓Y�����A�N�Z�X<br> *�i���ɋK�肪�Ȃ��ꍇ�̌v�Z�ʂƃ������g�p�ʂƂ��đz��ł�����́j* |
| - | ���p�萔����<br>(*amortized constant*) | [`std::vector::push_back`](/reference/vector/push_back.md) <br> *�i���܂ɔ��ɒ������Ԃ������邪�ʏ�͒Z�����ԂŊ������邽�߂ɁA���ϓI�ɂ͒萔���ԂƂ݂Ȃ�����́j* |
| $O\left(\log n\right)$ | �ΐ�����<br>(*logarithmic*) | ������͈͂̍Čv�Z<br> *�i�O�����C�e���[�^�v���𖞂����Ȃ��C�e���[�^�͈͂ɂ�鏉�����ɂ����郁�����Ċm�ہj* |
| $O\left(n\right)$ | ���`����<br>(*linear*) | �f�X�g���N�^�i�S�Ă̗v�f��j������K�v��������́j<br>�R�s�[�R���X�g���N�^<br>[`std::unordered_set` ���m�̓��l��r](/reference/unordered_set/unordered_set/op_equal.md) *�i���όv�Z���ԁj* |
| $O\left(n \log n\right)$ | ���`�ΐ�����<br>(*log-linear*) | [`std::sort`](/reference/algorithm/sort.md) <br> ��ʓI�� __����__ �Ƃ����\�[�g *�i���όv�Z���ԁj* |
| $O\left({n^2}\right)$ | ��掞��<br>(*quadratic*) | ��d���[�v<br>��ʓI�� __�x��__ �Ƃ����\�[�g *�i�ň��v�Z���ԁj*<br>[`std::unordered_set` ���m�̓��l��r](/reference/unordered_set/unordered_set/op_equal.md) *�i�ň��v�Z���ԁj* |
| $O\left({n^c}\right), \exist c\ge 1$ | ����������<br>(*polynomial*) | ���d���[�v<br>�s��v�Z |
| ${2^O\left(n\right)}$ | �w������<br>(*exponential*) | *�i�x�����邽�ߎ��p�I�łȂ��j* |
| $O\left(n!\right)$ | �K�掞��<br>(*factorial*) | *�i�x�����邽�ߎ��p�I�łȂ��j* |


## �R���e�i�̌v�Z��

�i���M���j

�����ł́A�������Ċm�ۂ��N����Ȃ��ꍇ�̒ʏ�̌v�Z�ʂ��L�ڂ���B�����ȏ����ɂ��ẮA�ʃy�[�W���Q�Ƃ��邱�ƁB

`std::stack` �A `std::queue` �A `std::priority_queue` ���̃R���e�i�A�_�v�^�̌v�Z�ʂ́A���������̌v�Z�ʂɏ�����B

| �R���e�i | N�v�f�̏����� | �R�s�[ | �擾 | �擪 | ���� | ���� | �}�� | �폜 | 
|---|---|---|---|---|---|---|---|---|
| [`array`](/reference/array.md) <a href="site-1">[^1]</a> | | | | | | | | |
| [`vector`](/reference/vector.md) | | | | | | | | |
| [`deque`](/reference/deque.md) | | | | | | | | |
| [`list`](/reference/list.md) | | | | | | | | |
| [`set`](/reference/set.md) | | | | | | | | |
| [`unordered_set`](/reference/unordered_set.md) | | | | | | | | |
| [`multiset`](/reference/multiset.md) | | | | | | | | |
| [`unordered_multiset`](/reference/unordered_multiset.md) | | | | | | | | |
| [`map`](/reference/map.md) | | | | | | | | |
| [`unordered_map`](/reference/unordered_map.md) | | | | | | | | |
| [`multimap`](/reference/multimap.md) | | | | | | | | |
| [`unordered_multimap`](/reference/unordered_multimap.md) | | | | | | | | |

- <a name="site-1"></a>[^1]: `std::array` �� `swap` �̌v�Z�ʂ��萔���ԂłȂ����߁A�R���e�i�̗v���𖞂����Ȃ��i����ȊO�̃R���e�i�́A�S�Ē萔���Ԃł���j�B


## �A���S���Y���̌v�Z��

�i���M���j
