# grid-dragndrop
그리드 - 드래그 앤 드롭 타입
 (c) 2019 김근애
   All rights reserved.

   @license oceco@naver.com

   arrStructure = [
       {
           "Index": 0, // 번호
           "View": true, // 컬럼 보기 or 숨기기
           "Fixed": true, // 컬럼 고정 or 유동
           "Name": "CheckName", // 컬럼명
           "Width": 50, // 컬럼 너비
           "Absolute": true // 컬럼 절대고정, 절대보기 여부
       }
       ...
   ]

   var instance = new TableGridAlign('id', {
       initArr: initArr,
       arr: arr,
       renderAfter: function (arr) {
           console.log('초기 렌더 이후');
           console.log(arr);
       },
       alignAfter: function(arr){
           console.log('사용자지정보기 확인 클릭 이후');
           console.log(arr);
       }
   });
