素材库使用说明
================

将全景照片 / 平面图 / 户型图文件放入本目录的 files/ 子目录，
然后运行 `npm run gen-library` 生成索引文件 index.json，
即可在应用的「素材库导入」中选择使用。

示例：
  public/library/files/客厅-20261001.jpg
  public/library/files/6F平面图.png

未来接入云服务器或 NAS：
  修改 src/utils/assetSource.ts 中的 listAssets / fetchAsset 两个函数为 API 调用即可，
  界面无需改动。
