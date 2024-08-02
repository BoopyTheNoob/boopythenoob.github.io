---
layout: default
---

# Cơ chế tự thiết lập thị trường với tích không đổi (Constant Product Automated Market Maker - CPAMM)

Nhằm hiện thực hóa tầm nhìn tiền tệ không lệ thuộc vào chính phủ, nhiều người trên thế giới đã thiết kế tiền điện tử và các hệ thống giao dịch chúng (chẳng hạn như [Ethereum](https://en.wikipedia.org/wiki/Ethereum) là một loại tiền điện tử và [Uniswap v2](https://en.wikipedia.org/wiki/Uniswap) là một hệ thống có thể giao dịch Ethereum). Trong bài viết này ta sẽ thảo luận, trên phương diện toán tài chính, về cách hệ thống như Uniswap v2 hoạt động thông qua cơ chế CPAMM như thế nào.

## Cơ chế tự thiết lập thị trường


## Bể thanh khoản với tích không đổi
Xét hai loại tiền tệ $$X$$ và $$Y$$ trên một hệ thống giao dịch, với số lượng của mỗi loại tiền tệ tại thời điểm $$t$$ nào đó lần lượt là $$X_t$$ và $$Y_t$$. Mô hình tích không đổi có nghĩa rằng tại mọi thời điểm, ta phải có tích
$$X_tY_t=C$$
với hằng số $$C$$ nào đó. Tổng quan hơn mô hình tích không đổi, ta có thể giới thiệu thêm một hằng số $$\alpha\in(0,1)$$ vào bên trong tích nói trên và được
$$X_t^{\alpha}Y_t^{1-\alpha}=C.$$
Ta sẽ thực hiện các tính toán trên trường hợp tổng quát này. Có thể nhanh chóng nhận xét rằng khi $$\alpha=\frac{1}{2}$$ ta có được mô hình tích không đổi (chính xác hơn là trung bình nhân), được đề cập đến trong sách trắng của Uniswap v2.

## Tỷ giá hối đoái và cách lập hợp đồng giao dịch
Giả sử tại thời điểm $$t$$, ta muốn thực hiện giao dịch một lượng $$\Delta Y_t=Y_t-Y_{t^-}$$ đơn vị tiền tệ $$Y$$ sang $$\Delta X_t=X_t-X_{t^-}$$ đơn vị tiền tệ $$X$$, khi đó để thị trường có 