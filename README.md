# Membuat-Aplikasi-Stosk-Barang


  <select>
                        <?php
                        $ambilsemuadatanya = mysqli_query($conn, "select * from stock");
                        while($fetcharray = mysqli_fetch_array($ambilsemuadatanya)){
                            $namabarangnya = $fetcharray['namabarang'];
                            $idbarangnya = $fetcharray['idbarang'];
                        ?>
                        <option value="<?php=$idbarangnya;?>"><?php=$namabarangnya;?></option>
                        <?php    
                        }
                        ?>
                    </select>