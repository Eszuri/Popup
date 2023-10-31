# Popup

-- html nya ---

<!DOCTYPE html>
<html lang="en">
<head>
     <meta charset="UTF-8">
     <meta name="viewport" content="width=device-width, initial-scale=1.0">
     <meta http-equiv="X-UA-Compatible" content="ie=edge">
     <title>Document</title>
     <style>
          body,p,h1 {
          margin: 0;
          }

          section {
          position: fixed;
          left: 50%;
          top: 50%;
          transform: translate(-50%,-50%);
          background-color: rgba(0,0,0,0.5);
          height: 0%;
          width: 0%;
          display: flex;
          justify-content: center;
          align-items: center;
          overflow: hidden;
          transition: 700ms;
          }

          div {
          width: 310px;
          height: 350px;
          background-color: white;
          border-radius: 3px;
          text-align: center;
          position: relative;
          padding-top: 20px;
          border: 4px solid black;
          color: black;
          }

          img{
          width: 80%;
          }

          div>h1 {
          position: absolute;
          cursor: pointer;
          right: 10px;
          top: 5px;
          }

          .att{
          text-transform: uppercase;
          font-weight: 900;
          font-size: 24px;
          }

          .att2 {
          width: 85%;
          margin: 10px auto 0 auto;
          font-weight: 700;
          text-align: left;
          }

          ul {
          margin-top: 15px;
          text-align: left;
          }
     </style>
</head>
<body>
     <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Nisi deleniti, quibusdam inventore nulla sit recusandae unde enim ipsum dolorum, voluptates illo in, iure quos debitis modi rem. Eligendi magni vel velit expedita omnis, ab illum non adipisci odio rem itaque facilis aliquam totam ut obcaecati quaerat laboriosam, maiores voluptates. Facilis, molestias accusamus sed pariatur quidem reprehenderit perspiciatis asperiores ad tenetur vel voluptatum, porro quae magnam suscipit repellat blanditiis tempore, expedita. Nobis tenetur dicta architecto animi sint distinctio obcaecati amet blanditiis impedit, illo praesentium libero laborum. Ratione voluptates consectetur beatae, atque, sequi ab recusandae, porro ducimus ipsam consequuntur vero! Dignissimos, suscipit.
     </p>
     <section>
          <div>
               <h1>X</h1>
               <img src="./1.jpg" alt="gambar">
               <p class="att">
                    Perhatian!
               </p>
               <p class="att2">
                    Saat ini bot sedang mengalami lonjakan user yang terlalu tinggi, sementara semua fitur dikunci dan hanya dapat digunakan oleh member Premium dan VIP
               </p>
               <ul>
                    <li>
                         Premium: 10K/Bulan
                    </li>
                    <li>
                         Grup VIP: 20K/Bulan/Grup
                    </li>
                    <li>
                         Ketik !premium di nomor bot untuk memesan
                    </li>
               </ul>
          </div>
     </section>
     <button>Click Guwe</button>
     <script>
          const btn = document.querySelector("button");
          btn.style.width = "200px";
          btn.style.height = "100px";
          btn.style.position = "fixed";
          btn.style.left = "50%";
          btn.style.top = "50%";
          btn.style.zIndex = "-1"
          btn.style.transform = "translate(-50%, -50%)";

          btn.addEventListener("click", ()=>{
          document.querySelector("section").style.width = "100%";
          document.querySelector("section").style.height = "100%";
          });

          document.querySelector("h1").addEventListener("click", ()=>{
          document.querySelector("section").style.width = "0%";
          document.querySelector("section").style.height = "0%";
          })
     </script>
</body>
</html>
