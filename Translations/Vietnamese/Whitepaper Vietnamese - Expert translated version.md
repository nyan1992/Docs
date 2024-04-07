Morpheus
Một Mạng Lưới tăng cường các Smart agents* (Đại lý thông minh)
*Smart agents là các dịch vụ được kết nối với blockchain, sử dụng các dữ liệu và chức năng off-chain để hỗ trợ các hành động on-chain. Điều này cho phép tích hợp hệ thống bên ngoài vào blockchain

Viết bởi Morpheus, Trinity, & Neo
Được xuất bản - ngày 2 tháng 9 năm 2023 
Liên kết tới Chi tiết kỹ thuật của Yellow Paper: https://github.com/MorpheusAIs/Docs/blob/main/YellowPaper.md

1. Giới thiệu
Morpheus được thiết kế để khuyến khích mạng ngang hàng (P2P) đầu tiên của Trí tuệ nhân tạo cá nhân thực hiện các Hợp Đồng Thông Minh thay mặt cho người dùng, được gọi là Đại Lý Thông Minh. Việc cung cấp cho người dùng các Đại Lý Thông Minh mã nguồn mở để kết nối với ví Web3, Dapps, và các hợp đồng thông minh hứa hẹn mở ra thế giới Web3 cho mọi người.
Ví Web3 của người dùng được sử dụng để quản lý khóa và ký giao dịch được đề xuất khi tương tác với các Đại lý thông mình. Một Mô hình Ngôn ngữ Lớn được huấn luyện trên dữ liệu Web3 bao gồm Blockchain, Ví, Dapps, DAOs và Hợp đồng Thông minh. Thuật toán SmartContractRank đánh giá và đề xuất các Hợp Đồng Thông Minh tốt nhất cho người dùng. Bộ nhớ dài hạn về dữ liệu người dùng và các ứng dụng kết nối được lưu trữ cục bộ hoặc qua đám mây phi tập trung để cung cấp bối cảnh rộng hơn cho các hành động của Đại Lý Thông Minh.
Cuối cùng, người dùng bình thường có thể trò chuyện với Đại Lý Thông Minh của họ bằng ngôn ngữ thông thường và có thể cho nó hiểu câu hỏi và thực hiện một hành động dựa trên ý định/phê duyệt của họ. Thời điểm này tương tự như khi công cụ tìm kiếm của Google đã đem Internet sơ khai đến với công chúng thông qua giao diện web dễ sử dụng vào cuối những năm 1990.
Để mọi người có thể truy cập Đại lý thông minh và tăng cường sự phi tập trung của cơ sở hạ tầng, chúng tôi đề xuất phát triển mạng lưới Morpheus. 
Mạng lưới Morpheus sẽ phát hành token một cách công bằng (token "MOR") để khuyến khích sự phát triển của tất cả bốn nhóm đóng góp chính cho mạng lưới. Cụ thể là, cộng đồng những người xây dựng giao diện, các lập trình viên đóng góp cho phần mềm/đại lý Morpheus, các nhà cung cấp vốn tạo thanh khoản và những người cung cấp dịch vụ tính toán, lưu trữ và băng thông. Lịch sử của Bitcoin và Ethereum đã chứng minh rằng sự cạnh tranh mở và tự do cho các token mã hóa khan hiếm có thể cung cấp cơ sở hạ tầng có thể mở rộng cho một blockchain công cộng trong thời gian dài.

<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/59PXm59X/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-001.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-001"/></a><br/><br/>

2. Bối cảnh & Lịch sử
Các công ty hiện tại như OpenAI, Microsoft và Google đều đang vận hành các mô hình ngôn ngữ lớn với mã nguồn đóng và thu phí sử dụng từ khách hàng và khai thác kinh doanh dữ liệu của họ. Các mô hình này bị kiểm duyệt, không an toàn và hoạt động trong các hệ thống kín. Nhu cầu cho một mô hình ngôn ngữ lớn với mã nguồn mở có sẵn miễn phí là rất lớn.  Llama, Falcon và các LLM nguồn mở khác đã được phát hành gần đây và đang nhanh chóng tiếp cận độ chính xác của các đối thủ cạnh tranh nguồn đóng của họ.
Những gì các mô hình ngôn ngữ lớn với mã nguồn mở này hiện đang thiếu là một giao diện đồ họa tiêu chuẩn mà người dùng có thể trò chuyện với chúng, một API cho các nhà phát triển, một giải pháp đám mây để di chuyển giữa các thiết bị và một cách để quản lý dữ liệu người dùng và quy trình phục hồi. Đây là lúc giao thức Đại lý Thông minh xuất hiện vì nó cung cấp LLM nguồn mở chạy cục bộ và được quản lý bởi ví Web3 của người dùng. .
Tuy nhiên, cách tiếp cận duy nhất cục bộ vẫn thiếu API cho các nhà phát triển xây dựng trên nó và giải pháp đám mây nơi một mạng lưới người dùng có thể chạy phần mềm trên phần cứng mạnh để kích hoạt các trường hợp sử dụng của các khách hàng có nhu cầu sử dụng ít, khi mà họ không cần phải tải xuống toàn bộ node hoặc Đại Lý Thông Minh cục bộ.


3.Tìm hiểu Morpheus

Morpheus sẽ cung cấp các APIs này và các chức năng đám mây phi tập trung bằng cách khởi chạy mạng lưới và phát hành token để thưởng cho những ai cung cấp cơ sở hạ tầng blockchain công cộng này cho các Đại lý thông minh. Khi triển khai Giao thức đại lý thông minh, Morpheus tìm cách thu thập các tài nguyên cần thiết cho AI cá nhân dựa trên nguồn mở để phù hợp và qua đó vượt lên trên khả năng của các công ty công nghệ cung cấp mô hình GPT nguồn đóng hiện nay. 

Ngay từ đầu Morpheus có nhiều lợi thế. Là người thông thạo Web3, người dùng có thể mua hoặc bán tiền điện tử, gửi stablecoin, truy cập hợp đồng thông minh và sử dụng các dịch vụ Dapps và DeFi mà ngày nay không có LLM nào được kết nối. Các rào cản pháp lý mà các công ty tập trung phải đối mặt đã ngăn cản họ cung cấp những công cụ này cho người dùng, vì vậy mô hình của họ có thể chat về các nhiệm vụ nhưng không hành động dựa trên lợi ích người dùng trong bối cảnh Web3. Chạy trên cơ sở hạ tầng công cộng phi tập trung rẻ hơn so với việc trả phí sử dụng cho Chat GPT cho mỗi người dùng mới.
Morpheus là loại hình thay thế giống như Linux dành cho các nhà phát triển muốn có thể nhanh chóng phát triển các đại lý / LLM mới mà không mất phí. Người dùng có thể duy trì quyền sở hữu dữ liệu cá nhân hoặc doanh nghiệp của họ. Điều này tránh rò rỉ, hack và tấn công từ đối thủ cạnh tranh. Bằng cách khen thưởng các nhà lập trình vì đã đóng góp mã không chỉ cho Morpheus mà còn xây dựng các Đại lý chuyên biệt hơn, trải nghiệm kiểu App Store/Agent Store cho người dùng sẽ phát triển. Với sự ổn định của dữ liệu, các câu lệnh và lịch sử do người dùng sở hữu, Giao thức Đại lý Thông minh trở thành giải pháp tốt nhất cho khả năng tương tác trong thế giới LLM và Đại lý.


Cuối cùng, Morpheus có giao diện đồ họa cho người dùng và tận dụng Electron để cho phép cài đặt bằng một cú nhấp chuột giúp Morpheus trở thành AI nguồn mở đầu tiên vượt qua "bài kiểm tra Friedl" nổi tiếng. Đây là một ngưỡng đánh giá khi tính dễ sử dụng của một phần mềm giúp những người không có chuyên môn về kỹ thuật trong công chúng nói chung có thể tiếp cận được phần mềm đó.

4.Cơ cấu token và phần thưởng

Trong phương án của chúng tôi, Token của Morpheus (ký hiệu "MOR") được sử dụng cho việc này. MOR được phân bổ mỗi ngày theo tỉ lệ 24% cho cộng đồng, 24% cho vốn, 24% cho máy tính, 24% cho lập trình viên và 4% cho quỹ phòng vệ.

Điều này phản ánh thực tế rằng để Morpheus phát triển, nó cần những điều sau:

Cộng đồng - Những người lập trình tạo giao diện người dùng/công cụ và đưa người dùng vào hệ sinh thái Morpheus.

Vốn - Mang lại nguồn tài trợ cho các hoạt động tính toán và code.

Khả năng Tính toán - Cung cấp thiết bị và năng lực

Lập trình - Cung cấp nguồn lực để vận hành cộng đồng, vốn và tính toán.

Nguồn cung của MOR token được giới hạn ở mức tối đa 42.000.000. Việc phân phối nguồn cung này sẽ bắt đầu bằng việc cả bốn nhóm nêu trên có thể kiếm token bằng cách tham gia đóng góp công sức (lao động) được chứng nhận và bằng việc đóng góp cổ phần (vốn) cho mạng lưới. Không có hoạt động đào trước. Không bán token sớm. Chỉ sự phát hành token một cách công bằng mà thôi.
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/Fs77Cf1D/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-002.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-002"/></a><br/><br/>
Việc phát thưởng sẽ bắt đầu ở mức 14.400 MOR mỗi ngày và sau đó giảm dần 2,468994701 MOR mỗi ngày cho đến khi phần thưởng về 0 vào ngày thứ 5.833. Vào thời điểm đó (khoảng 16 năm nữa) nếu Morpheus được sử dụng rộng rãi thì các loại phí sẽ thay thế trở thành nguồn động lực chính. Phí trả cho người dùng cho dữ liệu của họ, phí cho nhà cung cấp máy tính, phí cho nhà cung cấp vốn và phí cho người lập trình.

Giới hạn nguồn cung 42 triệu token MOR. 14.400 token mỗi ngày được phân bổ đều giữa cộng đồng, vốn, hoạt động lập trình và tính toán.

3.456 token để tính toán. Bằng chứng về giao dịch cho các lệnh gọi API được phân phối.
3.456 token cho mã. Bằng chứng về mã đã được cam kết và sáp nhập vào kho lưu trữ Morpheus.
3.456 token làm vốn. Bằng chứng về lợi suất stETH đã đóng góp, 50% được hoán đổi lấy MOR và ghép với 50% còn lại để khóa AMM dưới dạng Thanh khoản thuộc sở hữu của Giao thức (PoL).
3.456 token cho cộng đồng. Bằng chứng về việc xây dựng các ứng dụng và công cụ giao diện người dùng thu hút người dùng. Phần còn lại dành cho tài nguyên bảo vệ: 576 token mỗi ngày cho mục đích đó.
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/DzdZ4LYy/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-003.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-003"/></a><br/><br/>

5.Tiện ích của token MOR

Mục đích ở đây là làm cho token MOR cung cấp nhiều tiện ích cho những chức năng của mạng Morpheus. Do đó, việc sử dụng token MOR cung cấp cơ chế kế toán on-chain để tính toán phần thưởng dựa trên việc sử dụng phần mềm thực tế.

Các nhà phát triển trả MOR cho các bên cho thuê để có được các chức năng vượt xa những gì phần cứng cục bộ có thể thực thi. Phần token MOR này trả tiền cho các lệnh gọi API Morpheus cho các ứng dụng phi tập trung sử dụng Giao thức tác nhân thông minh. Người dùng có thể trả MOR cho các Đại lý chuyên biệt do nhà phát triển phát hành. Đổi lại, các nhà phát triển có thể trả cho người dùng MOR để đào tạo dữ liệu cho LLM/Đại lý mới.

Tất cả các dự án đều trải qua các giai đoạn phát triển. Điều quan trọng là ngay từ đầu, các tài nguyên có tính thanh khoản như ETH sẽ được sử dụng để trả tiền cho các nhà phát triển và mua thiết bị. Ethereum đã làm điều tương tự khi họ tận dụng BTC từ cộng đồng của mình để trả tiền cho việc mã hóa ban đầu cho blockchain của họ. Sự khác biệt ở đây là Giao thức đại lý thông minh đã được phát triển và Morpheus đang triển khai một phiên bản để mở rộng phạm vi tiếp cận của nó, do đó không cần phải bán token cho cộng đồng trước khi dự án đi vào hoạt động. Mã token MOR sẽ chỉ được thưởng sau khi phần mềm hoạt động.
  a.Ngắn hạn: Tại thời điểm ra mắt


Vốn - Các nhà cung cấp vốn nhận được phần thưởng MOR được chia theo tỷ lệ số stETH mà họ đã đóng góp trên tổng số StETH đã được gửi vào.
Tính toán - Nhà cung cấp dịch vụ tính toán nhận được MOR khi trả lời những yêu cầu của người dùng 
Lập trình - Coder nhận được MOR cho những đóng góp của họ cho phần mềm Morpheus đã được hợp nhất.
Cộng đồng - Những người xây dựng cộng đồng nhận được MOR cho hoạt động front end, xây dựng công cụ, sử dụng dịch vụ và giá trị mà họ mang lại cho mạng Morpheus.
  b.Trung hạn: Khi MOR tăng lượng lưu hành rộng hơn
Vốn - Phát triển sự cân bằng giữa việc phát thưởng cho các khối và phí kiếm được 
Tính toán/bên cho thuê - Phát triển sự cân bằng giữa phần thưởng khối và phí kiếm được.
Lập trình viên - Phát triển sự cân bằng giữa phần thưởng khối và phí kiếm được.
Cộng đồng - Phát triển sự cân bằng giữa phần thưởng khối và phí kiếm được.
  c.Dài hạn: Khi MOR có tính thanh khoản lớn và nhu cầu sử dụng cao
Vốn - Phần lớn phần thưởng sẽ đến từ việc hưởng phí cho hoạt động cung cấp thanh khoản của ETH cho token MOR 
Tính toán - Phí trả cho các nhà cung cấp máy tính sẽ chiếm phần lớn phần thưởng của họ.
Lập trình viên - Phí dành cho lập trình viên sẽ chiếm phần lớn phần thưởng của họ.
Cộng đồng - Phí do người dùng trả sẽ mang lại phần lớn phần thưởng cho họ.

*Lưu ý rằng đây không phải là một kế hoạch thời gian. Nó chỉ là mô tả về mỗi giai đoạn trong vòng đầu tư. Có thể mất nhiều năm để cộng đồng phát triển và trưởng thành qua từng giai đoạn và phần thưởng sẽ hết hạn sau khoảng 16 năm. Lịch trình phân phối kéo dài này nhằm mục đích dành thời gian để các token được phân phát một cách rộng rãi trên toàn cầu. Ngoài ra, việc phần thưởng giảm dần hàng ngày trong nhiều năm giúp tất cả người tham gia có thời gian để đạt được quy mô và chuyển đổi từ phần thưởng được trợ cấp sớm sang hoạt động chỉ bằng phí họ kiếm được.
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/PJcrn4NK/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-004.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-004"/></a><br/><br/>
6.Số lượng phát thưởng tiếp nối của MOR

Kể từ khi Bitcoin ra mắt, mọi người đã tranh cãi về việc “điều gì sẽ xảy ra khi phần thưởng khối cuối cùng sẽ dừng lại?” Để tránh cuộc tranh luận vô ích này trong bối cảnh Morpheus và để tiếp tục gắn kết các lập trình viên, cộng đồng, nhà cung cấp máy tính và vốn mới trong tương lai, chúng tôi đề xuất kế hoạch "Phát thưởng tiếp nối" token MOR. Việc phân phát tiếp nối MOR này sẽ bắt đầu sau khi token MOR cuối cùng được phân phát vào ngày thứ 5.833 của lịch phân phối.

Lượng phân phát tiếp nối sẽ được tính bằng cách xem xét số lượng token MOR đã đốt trong 5.833 ngày qua và đặt giá trị phân phát tiếp nối là 50% số lượng đã đốt. Giá trị phân phát tiếp nối này sẽ được phát ra trong khoảng thời gian 5.833 ngày tiếp theo. Nhưng trong mọi trường hợp, lượng phân phát ở đuôi sẽ không lớn hơn 16% lượng MOR đang lưu hành lúc đó.

Ví dụ: nếu trung bình 25% token MOR bị đốt trong 5.833 ngày đầu tiên thì 10.500.000 MOR sẽ bị đốt trong lịch trình phát hành đầu tiên. Sau đó, bằng cách áp dụng giá trị phân phát tiếp nối 50%, chúng tôi tính toán được 5.250.000 MOR có thể được thưởng trong khoảng giai đoạn 5.833 ngày lần thứ hai. Con số này chiếm khoảng 16,6% trong số 31.500.000 MOR còn lại đang lưu hành. Theo đó, số tiền này sẽ tiếp tục giảm xuống còn 5.040.000 MOR (16% số token đang lưu hành) để được thưởng trong khoảng thời gian 5.833 ngày tiếp đó hoặc tương đương 864 MOR mỗi ngày.

Sau khi hoàn tất giai đoạn 5.833 ngày lần thứ hai, quá trình này sẽ lặp lại. Lượng phân phát tiếp nối tiếp theo sẽ được tính toán lại bằng cách xem xét số lượng token MOR đã đốt trong 5.833 ngày trước đó và đặt giá trị phân phát tiếp nối là 50% số lượng đã đốt. Giá trị phân phát tiếp nối này sẽ được phát ra trong khoảng thời gian 5.833 ngày tiếp theo. Nhưng trong mọi trường hợp, lượng phân phát ở đuôi sẽ không lớn hơn 16% lượng MOR đang lưu hành khi đó.

Ví dụ: một lần nữa nếu 25% token MOR bị đốt trong giai đoạn thứ hai, thì tương đương với 9.135.000 MOR bị đốt trong lịch phát hành thứ hai. Sau đó, 4.567.500 MOR có thể được thưởng trong giai đoạn 5.833 ngày lần thứ ba. Tuy nhiên, vì con số này chiếm hơn 16% trong số 27.405.000 MOR còn lại đang lưu hành nên nó sẽ giảm xuống còn 4.384.800 MOR để phù hợp với phần thưởng hàng năm 1% (so với số token đang lưu hành).

Quá trình này lặp đi lặp lại mãi mãi trong tương lai.

Kết quả lâu dài là khoảng 1% phần thưởng MOR hàng năm (so với số lượng MOR đang lưu hành) sẽ dành cho các lập trình viên, hoạt động tính toán, cộng đồng và cung cấp thanh khoản trong tương lai.
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/gJg2NdWC/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-005.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-005"/></a><br/><br/>
*Lưu ý: Điều này không làm thay đổi bản chất của Giới hạn số lượng cung cấp cứng là 42 triệu MOR. Vì lịch phát hành đuôi theo định nghĩa chỉ là một phần token MOR đã bị đốt cháy, do đó token MOR chỉ có thể trở nên dần khan hiếm hơn với mỗi khoảng thời gian 5.833 ngày.
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/JzXtm9NX/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-006.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-006"/></a><br/><br/>
Hình này được cho thấy Đường cung thống nhất MOR hiển thị khoảng thời gian 5.833 ngày đầu tiên và cộng thêm lượng phân phát tiếp nối kéo dài từ năm 17 đến năm 256, dựa trên giả thuyết về tốc độ đốt trung bình 25% của MOR trong các kỷ nguyên.
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/QMrCM0my/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-007.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-007"/></a><br/><br/>
A. Cơ chế đồng thuận (bằng chứng) về Cộng đồng, Lập Trình, Sức mạnh tính toán & Vốn
Node đầy đủ Morpheus đi kèm với ví hoặc người dùng có thể kết nối ví hiện có của họ. Điều này cho phép người dùng ký và gửi các giao dịch do Smart Agent của họ đề xuất. Vì vậy, người dùng sẽ có thể tham gia kiểm chứng thông qua phần mềm Morpheus. Tuy nhiên, chẳng hạn, những người cung cấp vốn không bắt buộc phải sở hữu node đầy đủ. Họ có thể tương tác trực tiếp với Hợp đồng thông minh trên Ethereum/Arbitrum bằng cách sử dụng stETH.

B. Cơ chế đồng thuận (bằng chứng) về vốn và việc phát thưởng:
Định nghĩa của một nhà cung cấp vốn là người cung cấp stETH để tạo ra lợi nhuận cho mạng Morpheus, nơi sẽ trở thành Protocol-owned Liquidity (PoL = Thanh khoản giao thức sở hữu). Hợp đồng thông minh của nhà cung cấp vốn sẽ cung cấp 50% lợi tức stETH được tạo ra cho chức năng hoán đổi Morpheus. Hoán đổi mua token MOR từ Nhà tạo lập thị trường tự động (AMM), sau đó ghép chúng với 50% lợi nhuận stETH còn lại và khóa vào Nhóm thanh khoản AMM dưới dạng PoL. Điều này sẽ cung cấp tính thanh khoản cho tất cả các lập trình viên, người xây dựng cộng đồng và nhà cung cấp máy tính. Phí thu được từ trạng thái thanh khoản được tái đầu tư vào nhóm để đảm bảo tăng trưởng thanh khoản ổn định.

Bằng cách này, tất cả lợi nhuận kiếm được từ tiền gửi stETH của người dùng sẽ được chuyển đổi thành Thanh khoản sở hữu bởi giao thức (PoL). Lợi tức vẫn ở dạng PoL vô thời hạn, nhưng người dùng có thể rút stETH của họ bất cứ khi nào sau thời hạn khóa 7 ngày ban đầu. Nếu số stETH bị rút, phần thưởng MOR sẽ không còn được tích lũy.

Do đó, Nhà cung cấp vốn sẽ nhận được token MOR (được tính theo từng khối) được chia theo tỷ lệ đóng góp của họ so với tổng số stETH đã gửi. Ví dụ: nếu có 100 Nhà cung cấp vốn, mỗi người đóng góp 1 stETH vào ngày đầu tiên khi mạng ra mắt và tổng số vốn bằng 100 stETH, thì mỗi người sẽ nhận được 1% trong số 3.456 token MOR vào ngày này = 34,56 MOR.

Người ta đã đề xuất gọi quá trình đóng góp lợi nhuận, swap và bổ sung thanh khoản này là "TCM" từ viết tắt của"techno-capital machine" ("cỗ máy vốn - kỹ thuật") để vinh danh nhà triết học e/acc Beff Jezos.(https://twitter.com/BasedBeffJezos)

Xem link giải thích chi tiết về Techno Capital Machine tại đây: TCM (https://github.com/MorpheusAIs/Docs/blob/main/!KEYDOCS%20README%20FIRST!/TechnoCapitalMachineTCM.md)

C. Cơ chế đồng thuận (bằng chứng) lập trình, đăng ký và phần thưởng:

Định nghĩa của Coder là người đã tải xuống và chạy node Morpheus bản đầy đủ, kết nối ví của họ và đóng góp một đại lý, hợp đồng thông minh hoặc phần mềm khác cho Mạng Morpheus. Code phải tuân theo Hướng dẫn dành cho người viết code.(https://github.com/MorpheusAIs/Docs/blob/main/!KEYDOCS%20README%20FIRST!/Coder%20Guide.md)

Coder sẽ gửi giao dịch MOR tới Coder Smart Contract để đăng ký đại lý/hợp đồng thông minh hoặc phần mềm của họ. Bộ mã hóa sẽ đưa vào bản ghi nhớ giao dịch siêu dữ liệu sau.

a Liên kết IPFS tới endpoint phần mềm của họ trong trường ghi nhớ của giao dịch MOR khi họ đăng ký.
b Chữ ký được mã hóa, tương tự như cách nhà phát triển ký/xác thực các bản phát hành của một ứng dụng.
c. Số phiên bản của phần mềm.
d. Một mã hash về trạng thái của chương trình để người dùng có thể kiểm tra xem đây có phải là bản sao hợp lệ và không bị thay đổi hay không.

Những người đóng góp cho cơ sở code của mã Morpheus được chia thưởng theo tỉ lệ tương ứng với tổng đóng góp (được cộng dồn) đã thực hiện trên kho lưu trữ được đánh giá bằng hệ thống Full Time Equivalent (FTE). Ví dụ: nếu có 10 lập trình viên, mỗi người đã đóng góp 10% thời gian FTE (tính theo tỉ trọng) khi mạng khởi chạy thì mỗi người sẽ nhận được 10% trong số 3.456 mã thông báo MOR mỗi ngày = 345,6 MOR. Tính toán này được cập nhật mỗi tháng dựa trên sự đóng góp tích lũy về thời gian FTE (tính theo tỉ trọng) của phiên bản mainnet hiện tại của phần mềm Morpheus.

Khái niệm ở đây KHÔNG dựa trên Lý thuyết Giá trị Lao động. Không quan trọng là làm việc bao nhiêu giờ mà quan trọng là giá trị do công việc đó tạo ra. Đó là lý do tại sao chủ sở hữu kho lưu trữ phải thực sự hợp nhất mã (sản phẩm của phần công việc) để nó được tính vào phần thưởng. Chủ sở hữu kho lưu trữ đóng vai trò là "khách hàng" trên thị trường.

Nếu người đóng góp Mã yêu cầu quá nhiều trọng số cho Đóng góp hoặc chất lượng của đóng góp không thể đủ tiêu chuẩn hoặc có chất lượng thấp thì có khả năng nó sẽ bị chủ sở hữu kho từ chối. Và mặc dù bất kỳ ai cũng "có thể" tạo một kho lưu trữ nhưng phải mất rất nhiều công sức để duy trì và cũng thu hút mọi người đóng góp vào kho lưu trữ của bạn thay vì những người khác, vì vậy thị trường có thể tập trung vào các kho lưu trữ tốt nhất với nhiều người đóng góp và kết quả code tốt nhất.

Nguồn mở và kinh tế thị trường tự do sẽ giành chiến thắng.

Khi có các đại lý chuyên biệt, các công cụ hoặc chuỗi (các yêu cầu/truy vấn tới LLM) có thể tương tác với Morpheus, thì một nửa (50%) phần thưởng sẽ thuộc về các nhà phát triển của họ. Phần thưởng sẽ được tính tỷ lệ thuận với việc sử dụng các đại lý đó. Ví dụ: nếu có 10 nhà phát triển xây dựng 10 đại lý, mỗi tác nhân tạo ra 10% mức sử dụng đại lý trên mạng Morpheus. Hợp đồng thông minh Morpheus sẽ tính toán số liệu thống kê sử dụng đó thông qua các giao dịch MOR. Sau đó, các lập trình viên phần mềm Morpheus sẽ kiếm được 50% phần thưởng MOR và mỗi nhà phát triển của một đại lý chuyên biệt sẽ nhận được 5% số token = 172,8 MOR cho mỗi nhà phát triển trong ví dụ này.

Rất nhiều nghiên cứu hàng đầu đã được thực hiện trong lĩnh vực "Cơ chế đồng thuận/ Bằng chứng đóng góp" này là do những người giỏi tại TEA Protocol thực hiện. Bao gồm Max Howell, nhà phát triển Home Brew. Nhiều thông tin thêm có thế được tìm thấy ở đây. Morpheus có thể xem xét tận dụng TEA sau khi ra mắt vào năm 2024.
D. Cơ chế đồng thuận tính toán & phần thưởng:

Nhà cung cấp khả năng tính toán được định nghĩa là bất kỳ thực thể nào chạy node đầy đủ cung cấp tài nguyên về sự tính toán, có địa chỉ MOR và đấu thầu IPS (suy luận mỗi giây, đơn vị suy luận nguyên tử trong AI) thông qua Router. Khi Nhà cung cấp thắng thầu, nó sẽ cung cấp tài nguyên tính toán (GPU, v.v.) cho các mô hình AI khác nhau cho người dùng. Các nhà cung cấp cần phải chứng minh rằng họ có LLM nhất định, bằng cách ký hash của mô hình LLM bằng khóa của họ. Nhà cung cấp máy tính CHỈ được thanh toán khi có nhu cầu về việc sử dụng khả năng tính toán của họ. Điều này ngăn chặn tình trạng phần lớn MOR được phát ra sớm khi mạng không cần đến.

Để đủ điều kiện nhận các yêu cầu Tính toán, địa chỉ của Nhà cung cấp Điện toán phải đang nắm giữ token MOR để ngăn chặn các cuộc tấn công Sybil.

Loại phần cứng của nhà cung cấp không ảnh hưởng đến mạng, miễn là chúng đáp ứng bài kiểm tra Đạt/Không đạt của Người dùng. Bất kỳ Nhà cung cấp nào đấu thầu cho nhiều Truy vấn hơn mức họ có thể xử lý một cách hiệu quả sẽ bị phạt do không thực hiện được bài kiểm tra này.

Router (Bộ định tuyến) là một ứng dụng phần mềm có địa chỉ MOR và đàm phán 2 mặt của thị trường giữa Người dùng và Nhà cung cấp. Router đăng ký và theo dõi địa chỉ và sự đấu thầu của Nhà cung cấp, xử lý Yêu cầu từ Người dùng, ghi lại [mili giây] và kiểm tra Đạt/Không đạt của các Yêu cầu đã xử lý, đồng thời hướng dẫn Hợp đồng Tính toán ghi có cho Nhà cung cấp đủ điều kiện để thanh toán bằng MOR khi được yêu cầu. Router không bao giờ gửi hoặc nhận các giao dịch MOR (cũng như các giao dịch trên bất kỳ blockchain nào). Router không bao giờ nhìn thấy nội dung của Yêu cầu cũng như phản hồi.

Quy trình làm việc
Người dùng, Nhà cung cấp và Router đều tạo khóa pub MOR (đây là danh tính của họ và tất cả các tin nhắn đều được ký như vậy).
Nếu Người dùng giữ bất kỳ số dư MOR nào, Người dùng có thể gửi thông báo Yêu cầu Tính toán “RFC” đã ký tới Router.
Router ưu tiên RFC dựa trên số dư MOR của Người dùng.
Router chọn Nhà cung cấp hỗ trợ [LLM], được ưu tiên dựa trên Giá thầu trên mỗi IPS thấp nhất tính theo MOR.
Router gửi kiểm tra hoạt động tới Nhà cung cấp. Nếu Đạt thì:
Router kết nối Người dùng với Nhà cung cấp qua TCP/IP.
Người dùng gửi Truy vấn ([LLM],[prompt]) tới Nhà cung cấp.
Nhà cung cấp tính toán Truy vấn, gửi Kết quả cho Người dùng.
Người dùng báo cáo các số liệu thành công cho Router (chẳng hạn như IPS đã nhận được hoặc thời gian thực hiện hoặc bỏ phiếu đạt/không đạt).
Router hướng dẫn Hợp đồng tính toán ghi có MOR cho Nhà cung cấp nếu công việc được hoàn thành thỏa đáng.
(Một thời gian sau) Nhà cung cấp yêu cầu thanh toán MOR từ Hợp đồng tính toán và Hợp đồng tính toán sẽ gửi thanh toán MOR nếu hợp lệ (TX blockchain đầu tiên cho đến hiện tại, có thể được chia theo đợt).
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/G2LpFtZP/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-008.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-008"/></a><br/><br/>
Khuyến khích cung cấp khả năng tính toán
Trong năm đầu tiên sau giai đoạn khởi động của Hợp đồng vốn, 100 nhà cung cấp khả năng tính toán hàng đầu có thể được hưởng tỷ lệ 2,4% lượng phân phát MOR. Điều này được tính toán bởi các Router và được tính trong hợp đồng điện toán.

Để biết thông tin chi tiết, hãy truy cập bài viết Mô hình tính toán Yellowstone (https://github.com/MorpheusAIs/Docs/blob/main/!KEYDOCS%20README%20FIRST!/Yellowstone%20Compute%20Model.md)

E.Cơ chế đồng thuận, lưu nhập và phần thưởng cho người xây dựng cộng đồng:
Định nghĩa của Người xây dựng cộng đồng là họ đã tải xuống và chạy node phiên bản đầy đủ của Morpheus, kết nối ví của họ và đang sử dụng API Morpheus để cung cấp giao diện người dùng và các công cụ của nhà phát triển. Những khoản đóng góp mà họ cung cấp có thể được tính bằng cách bao gồm giao dịch đã ký do Đại lý thông minh tạo ra cùng với kết quả đầu ra từ giao dịch MOR.

Người xây dựng cộng đồng sẽ gửi giao dịch MOR đến Hợp đồng thông minh của Người xây dựng cộng đồng để đăng ký điểm cuối API để nhận những truy vấn. Người xây dựng cộng đồng sẽ đưa vào bản ghi nhớ giao dịch siêu dữ liệu sau:

a. Liên kết IPFS tới giao diện người dùng hoặc công cụ của họ thông qua điểm cuối trong trường ghi nhớ của giao dịch MOR khi họ đăng ký.
b. Chữ ký đã mã hóa, tương tự như cách nhà phát triển ký/xác thực bản phát hành ứng dụng.
c. Mã số phiên bản của phần mềm Morpheus họ đang sử dụng.
d. Một mã hash trạng thái của giao diện người dùng / công cụ để người dùng có thể kiểm tra xem đó có phải là bản sao hợp lệ và không bị thay đổi hay không.

Tỉ lệ phí giao dịch MOR mà mỗi Người xây dựng cộng đồng đốt sẽ đóng vai trò là bằng chứng xác nhận về trạng thái của Người xây dựng cộng đồng và nhận được một phần token MOR mỗi ngày.

Ví dụ: nếu có 100 Người xây dựng cộng đồng vào ngày đầu tiên khi mạng ra mắt thì mỗi người sẽ nhận được phần thưởng theo tỷ lệ dựa trên số MOR mà họ đã đốt thông qua phí. Trong trường hợp này, giả sử mỗi người trong số 100 Người xây dựng cộng đồng đã đốt 100 MOR, vậy thì 1% của tổng số 3.456 token MOR mỗi ngày = 34,56 MOR.

6.Biểu đồ người dùng Morpheus
<a href="https://postimages.org/" target="_blank"><img src="https://i.postimg.cc/0jr2435b/Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-009.png" alt="Aspose-Words-2cf599d8-2dda-45f4-b1b0-62375945567c-009"/></a><br/><br/>
A.Phần thưởng Morpheus được phân phối bởi Hợp đồng thông minh trên L2 của Ethereum 
Việc gửi stETH để lấy phần thưởng sẽ được thực hiện trên mạng chính Ethereum, khi token Morpheus (MOR) được phát thưởng trên Arbitrum - một L2 của Ethereum, nhằm mục đích thanh toán và thực hiện các hoạt động liên quan đến tiện ích MOR khác.

Lưu ý rằng Morpheus không cần dành phần thưởng MOR cho cơ chế đồng thuận blockchain hoặc giao dịch nhờ việc xây dựng trên Ethereum và Arbitrum ở lớp thứ 2.

Người gửi tiền sẽ có thể gửi giao dịch đến Hợp đồng thông minh MOR và nhận phần thưởng MOR của họ bất cứ lúc nào. Họ cũng có thể rút stETH của mình bất cứ lúc nào.

B.Thị trường tự do đặt phí cho Morpheus

Các hệ thống tốt nhất tối thiểu hóa việc chọn các con số cố định và thay vào đó để thị trường tự do quyết định càng nhiều biến số càng tốt. Lệ phí là một ví dụ tuyệt vời về điều này. Thay vì chọn một khoản phí tùy ý để tính phí, Morpheus để lại những con số này cho người dùng, nhà phát triển, nhà cung cấp vốn và máy tính. Ví dụ: nếu nhà cung cấp khả năng tính toán có thể đưa ra mức giá 0,02 USD cho mỗi 1.000 IPS cho LLM của họ và người dùng quyết định trả mức giá đó thì đó là mức giá mà thị trường sẵn sàng trả. Khi tốc độ tính toán tăng lên, giá cả có thể sẽ thay đổi và do đó tốt hơn nên để những biến số này và các biến số khác cho những người sử dụng phần mềm Morpheus quyết định.

Phí tính toán
Số phí được đặt thông qua quy trình đấu thầu cạnh tranh giữa người dùng và nhà cung cấp khả năng tính toán. Thị trường mở phát triển theo thời gian. Thị trường tự do cung cấp khả năng tính toán thay vì ưu tiên cho cơ chế đồng thuận hoặc các node đặc quyền.

Phí lập trình / đại lý thông tin
Số phí do người lập trình đặt ra và được người dùng chấp nhận. Tùy chọn thanh toán phí và đốt token MOR với mỗi khoản phí. Thị trường mở phát triển theo thời gian. Thị trường tự do cho code thay vì sự đồng thuận về nhiệm vụ.

Phí cho việc cung cấp vốn
Số phí được đặt ra theo lượng phân phát MOR hàng ngày và được chấp nhận bởi người dùng muốn cung cấp vốn. Thị trường mở phát triển theo thời gian. Thị trường tự do về vốn thay vì sự đồng thuận về kho bạc.

Phí cho cộng đồng người dùng
Khoản phí do người dùng đặt ra và được người mua dữ liệu chấp nhận. Tùy chọn thanh toán phí và đốt token MOR với mỗi khoản phí. Thị trường mở phát triển theo thời gian. Thị trường tự do cho dữ liệu.

Tất cả các khoản phí đều được thanh toán bằng token MOR, tạo ra nhu cầu tự nhiên trong hệ thống khi mức sử dụng tăng lên.

B.Sử dụng việc phân phát thưởng để khuyến khích các đại lý trung thực và sửa chữa tổn thất trong trường hợp có lỗi

Một ứng dụng quan trọng khác của MOR & ETH trong mạng Morpheus sẽ là đền bù cho người dùng trong trường hợp Đại lý thông minh / Hợp đồng thông minh bị lỗi. Chúng tôi tin rằng việc quản lý và xây dựng danh tiếng được hỗ trợ bằng các nguồn lực kinh tế sẽ là chìa khóa để tăng cường niềm tin vào Đại lý thông minh và có nguồn tài trợ để giải quyết các lỗi và các vấn đề phát sinh khác. Sau một lỗi lớn và hậu quả là hard fork của Bitcoin vào năm 2010, một nhà phát triển có tầm quan trọng ban đầu tên là Gavin Andresen đã đứng ra trả Bitcoin cho những người khai thác đã mất phần thưởng do hard fork. Hành động này rất quan trọng và nhanh chóng giải quyết hard fork nhưng nó chỉ mang tính đặc biệt.

Nhận thức trước rằng phần mềm không bao giờ hoàn hảo Morpheus đang dành 4% tài nguyên MOR để trả nợ cho những người bị ảnh hưởng bởi một lỗi có thể xảy ra trong mã. Cộng đồng nhà phát triển Morpheus sẽ đóng vai trò nhận biết khi nào một lỗi hoặc lỗi có ảnh hưởng kinh tế đến người dùng, nhà cung cấp máy tính hoặc nhà cung cấp vốn. Các tài nguyên này sẽ dùng để chi trả cho một danh sách lỗi được xác định trước nhằm cho phép các lỗi trong Hợp đồng thông minh Morpheus hoặc cài đặt cục bộ.

Để bảo vệ rộng hơn, việc tích hợp với Nexus Mutual hoặc hợp đồng thông minh/mạng bảo vệ phi tập trung tương tự có thể được xem xét để giải quyết các trường hợp cận biên với các đại lý/hợp đồng thông minh muốn được đưa vào Morpheus Agent Store (Cửa hàng đại lý Morpheus) hoặc được xếp hạng tốt hơn theo thuật toán SmartContractRank.

Thông tin chi tiết về quỹ bảo vệ có tại đây (https://github.com/MorpheusAIs/Docs/blob/main/!KEYDOCS%20README%20FIRST!/Protection%20Fund%20Details.md)
C. Lưu trữ để duy trì và ví để phục hồi
Thay vì lưu trữ dữ liệu cá nhân trong chính mạng Morpheus, vốn có chi phí rất cao và là lực lượng tập trung, các cá nhân sẽ nắm giữ các khóa riêng kiểm soát quyền truy cập vào dữ liệu, lời nhắc và ví của họ. Bản thân dữ liệu sẽ được lưu trữ bằng tiêu chuẩn IPFS và mạng Filecoin để lưu trữ dài hạn phi tập trung. Có thể sắp xếp việc tận dụng Filecoin EVM và DeFi để mang lại bộ lưu trữ định kỳ vĩnh viễn. Ngoài ra, người dùng có thể trả phí lưu trữ theo kiểu ENS hàng năm. Cách tiếp cận này cho phép giữ ví Web3 riêng tư làm chìa khóa để di chuyển/khôi phục dữ liệu này sang các thiết bị khác nhau khi người dùng thay đổi máy tính hoặc điện thoại.


D.Các gói phát triển phần mềm Morpheus và hợp đồng thông minh
Thay vì lưu trữ dữ liệu cá nhân trên chính mạng Morpheus, vốn có chi phí rất cao và quản lý tập trung, các cá nhân sẽ nắm giữ các khóa riêng kiểm soát quyền truy cập vào dữ liệu, truy vấn và ví của họ. Bản thân dữ liệu sẽ được lưu trữ bằng tiêu chuẩn IPFS và mạng Filecoin để lưu trữ dài hạn phi tập trung. Có thể sắp xếp việc tận dụng Filecoin EVM và DeFi để mang lại bộ lưu trữ định kỳ vĩnh viễn. Ngoài ra, người dùng có thể trả phí lưu trữ theo kiểu ENS hàng năm. Cách tiếp cận này cho phép giữ ví Web3 riêng tư làm chìa khóa để di chuyển/khôi phục dữ liệu này sang các thiết bị khác nhau khi người dùng thay đổi máy tính hoặc điện thoại.

E.Ngăn xếp công nghệ, Hợp đồng thông minh & sự phát triển của Morpheus
Việc triển khai Morpheus của Giao thức Đại lý Thông minh sẽ là một nhánh trực tiếp của kho lưu trữ được chạy cục bộ hiện có. Thay đổi quan trọng nhất sẽ là cập nhật SmartContractRank để bao gồm kiến thức về token MOR và các chức năng của nó trong việc cung cấp một mạng lưới Đại lý thông minh.

Token Morpheus MOR đang được phát triển dưới dạng Hợp đồng thông minh trên Ethereum thông qua tiêu chuẩn ERC20 dành cho các token có thể thay thế được. Hầu hết các hợp đồng thông minh đều dựa trên Ethereum và Ethereum Virtual Machine đã trở thành ngôn ngữ chung của Web3. Để giảm chi phí gas khi gửi phần thưởng hàng ngày, Morpheus sẽ tận dụng lớp 2 của Ethereum có tên là Arbitrum.

Việc lựa chọn mạng Ethereum là nơi khởi đầu tốt nhất do các thao tác on-chain như stake ETH chỉ có thể được xác thực bằng hợp đồng thông minh chạy trên cùng mạng. Ngoài ra, việc xác thực mã hóa on-chain thông qua tên miền ENS hoặc địa chỉ ví Ethereum còn bổ sung thêm một phương tiện kết nối mã khác được đóng góp vào ví của lập trình viên đã cung cấp nó. Một bản ghi mà Hợp đồng thông minh Morpheus có thể truy cập hàng ngày.

Ngoài ra, bằng chứng ZK (không kiến thức) về khả năng mở rộng và quyền riêng tư là chìa khóa cho nhiều trường hợp sử dụng. Vì vậy, bắt đầu với những khả năng này, ngày đầu tiên sẽ đưa cộng đồng Smart Agent vào vị trí tốt nhất cho tương lai. Arbitrum đang trong quá trình bổ sung công nghệ ZK với phần lớn trong số đó đã được đưa vào.

Trong thời gian tới, lựa chọn ngăn xếp công nghệ này đảm bảo Morpheus trực tiếp nằm trong lớp bảo mật của L1 Ethereum với chi phí gas giảm của lớp hai. Trong trung hạn, lựa chọn này cũng cung cấp một lộ trình để mở rộng Morpheus sang các L2 khác của Ethereum và các mạng tương thích EVM khác.

Khi khả năng tương tác giữa các mạng được cải thiện, Morpheus sẽ tìm cách phục vụ tất cả các nhà xây dựng AI Agent trên Web3 ở khắp các cộng đồng nhà phát triển tương thích  với EVM/ Solidity. Chúng tôi ghi nhận các cộng đồng xây dựng mạnh mẽ trên Arbitrum, Polygon, OP Stack, Base, Arbitrum, Avalanche, Polkadot, Solana, Filecoin & Cosmos có chung tầm nhìn và giá trị. Morpheus ngày nay chỉ có thể thực hiện được nhờ các công cụ được các nhà phát triển xây dựng trên những mạng này.

F.Bảo mật dữ liệu người dùng
Để tránh rò rỉ dữ liệu riêng tư khi gửi truy vấn tới mạng ngang hàng Morpheus của Các Nhà cung cấp khả năng tính toán, phần mềm nên tìm cách tận dụng các phiên bản Mã hóa đồng hình hoàn toàn (FHE) của Mô hình ngôn ngữ lớn khi chúng được phát hành. Ngoài ra, với sự ra đời của khả năng tăng tốc phần cứng cho FHE vào năm 2024/2025, dự kiến chi phí cho tính toán này sẽ ngang bằng với xử lý văn bản thuần túy.

Ví dụ về LLM https://huggingface.co/blog/encrypted-llm
Ví dụ về EVM https://www.fhenix.io/


G.Sự bắt đầu của mạng lưới và thời gian khởi động 90 ngày
Mạng Morpheus bắt đầu với phiên bản cài đặt cục bộ 0.0.1, sau đó tiếp tục với hợp đồng thông minh token MOR và sau đó là phần mềm phiên bản đầy đủ của node.

Các hợp đồng thông minh tính toán phần thưởng MOR phải được thử nghiệm rộng rãi thông qua testnet (mạng thử nghiệm) trước khi triển khai lên mainnet (mạng chính).

Ngoài ra, sẽ có một sự trì hoãn 90 ngày diễn ra 1 lần duy nhất (được gọi là thời gian khởi động) từ khi mạng chính bắt đầu tính toán phần thưởng cho đến khi người dùng có thể nhận/gửi những token MOR đó. Giai đoạn khởi động này sẽ đảm bảo có đủ token MOR sẵn sàng để lưu hành nhằm thực hiện các chức năng tiện ích của mạng.

Để khởi động AMM, 4% token MOR dành riêng cho quỹ bảo vệ (51.444 MOR trước ngày thứ 90) sẽ được sử dụng cho mục đích này.

Các bước này sẽ đảm bảo rằng 1.286.111 MOR có thể được rút ra vào đầu ngày thứ 91 trên mạng chính và do đó tránh tình trạng khan hiếm token cực độ như đã xảy ra với sự ra mắt của Zcash, khi chỉ có một số token lần đầu tiên có sẵn kể từ ngày khai thác đầu tiên. Vấn đề này đã khiến thị trường phải mất nhiều tuần để đạt được trạng thái cân bằng và thiết lập giá hợp lý. Morpheus tránh được vấn đề này với khoảng thời gian khởi động 90 ngày, qua đó chuẩn bị đủ nguồn cung token đủ để đáp ứng tiện ích của nó và đạt đến mức giá hợp lý.

Sau khi token MOR có thể được rút và gửi thì Mạng Morpheus có thể cho phép các giao dịch MOR thanh toán cho các lệnh gọi API, đại lý tùy chỉnh và xác thực Cổ phần của những người tham gia trong mạng.

7.Kết luận
Chúng ta đang đến gần một thời điểm quan trọng trong lịch sử. Với Morpheus, mọi người sẽ có một AI cá nhân mạnh mẽ có khả năng suy nghĩ cùng họ và thực hiện các hành động có lợi cho họ. Giống như cách máy tính cá nhân và công cụ tìm kiếm trao quyền cho cá nhân, ngày nay chúng ta cũng có cơ hội tương tự với AI cá nhân. Giao thức Đại lý Thông minh đem lại sự kết hợp hài hòa giữa các khả năng của LLM, Các Đại lý và Web3. Morpheus mở rộng những khả năng đó thành một mạng công cộng có khả năng đẩy nhanh việc phân phối và sử dụng hàng loạt Đại lý thông minh.

Chúng tôi tin rằng các biện pháp khuyến khích mang tính kinh tế là cách tốt nhất để chúng tôi đảm bảo kết quả tốt nhất từ sự ra đời của AGI. Hãy giúp chúng tôi đảm bảo một tương lai của nguồn mở, không cần cấp phép và tự do cho mọi người.

8.Bối cảnh về sự ra đời của Morpheus:
Tôi nhận được email từ nhà phát triển có tên Morpheus vào ngày 2 tháng 9 năm 2023 với đề xuất trên.

David,

Bên dưới là đề xuất ra mắt "Morpheus - Mạng lưới hỗ trợ các đại lý thông minh".

Bài viết  soạn ra tokenomics, ngăn xếp công nghệ và các cách tính toán cơ chế trao thưởng công bằng cho cộng đồng, lập trình viên, nhà cung cấp vốn và cung cấp khả năng tính toán bằng token.

Bài viết này được cung cấp miễn phí cho cộng đồng Smart Agent và có sẵn trên trang công cộng.

Hãy giải phóng tâm trí của bạn.

Morpheus


